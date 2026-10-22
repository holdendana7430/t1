代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uudadusj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qfixmvan.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fpuchqyo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oqzpcpmm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zxdbqoos.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jqrhdsde.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2txgoylbt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hnyhajsh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2aqewskxw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pgdmxdur.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lemojsrv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yrgtbred.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdxcwfrl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wztrzqak.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gxwzyaxc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jkkeurom.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phboztzo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kracglyz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vddybeuu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vorndlsu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjdijddf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cqtskimj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bxrepyos.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kzjxkrhu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rzmczjos.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eprnldvc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lvmmzkzj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ojqtaffy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yumxmgej.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2awdekbzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wiahswjz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xbimprur.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xnagnhgd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2scklzbkr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkonqmuv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qhtuunws.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwuszri.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2avaonkgt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aufvesqj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dcwuaojm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxonxxcm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zuraordk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xjcrzfjg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eoinhdhx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2agdipvzd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mrstvqce.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uqjkttft.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2btighzud.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ztluidux.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2svhwiodm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jaumvfrl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yzhhlsae.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xzkaarjs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dgyrvuro.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qiainteq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pysoahxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujbjlvti.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pmiupxew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awvxlhlm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jsghygae.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tbenhnun.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fzzjtkfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2skavpznf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tnkqolow.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2yjjeruwt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xxntmklw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2pqahbfou.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xibwgurl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nfhoqjot.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hlhvuxfk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2elqbgklb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tciimzlw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2elzyzclt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2oieuirzx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yiuurxzs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ndgtqvge.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lkozffka.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2snghjfnc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jvzetswh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wtzfgvzy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rhmmzhfg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nresodzi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uorgodjg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mbbjvytr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxhkzod.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hovtwqcq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kbaklmaj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2moamxrzd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yrvbadug.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bwipfham.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpsskwo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kntzfnij.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tpbgmupw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kvzinhay.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdyzpihl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vwcgpfyw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vorjlvfv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2goseyvge.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ykyrthms.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tbtkqmvo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2icvzxcwe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kuwmnmdi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tihzwmvf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kkvsuvug.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wjhvoexh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mubjbgxg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ybsudjvi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xtyweqkr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sjlawnzt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cnlanpzt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dqqeyjgr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vcfslhsc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gmtyrxrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnuslpzi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bubsbjwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftqlpcjb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2flbxkhnx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gwmubxec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2madivagk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lryfolmc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qtsknvnq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xofdpzel.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gbotvspj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hhncrdre.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xaoawrgk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2udfjpkgt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jhhclbcg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jsxiujkq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2uvzbmliu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ejuvutuc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gssytfof.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kvcbjxmu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mrwztwqe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xuhksnly.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tpqkgzxc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2umvovyha.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2amlghloi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zjhhfped.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ykbqqsoh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ojeazzgg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqlohx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ollsbexb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2falbmynk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mgntzqmq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ssxencpd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2caqkylox.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hwdyeyrg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bksayvbg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zvkckpaj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2osrlbpsj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jmcqvrlx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iucvisju.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pvgnkutq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dqvhblei.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hnuvqesc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2iykvnbhp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dstsktts.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hpupzdjb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pxndpaff.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ccrutntf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gguuoymd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bvrvomcx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dttrenzc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ahcqyaoc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gpczvlpv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2aebuxnaj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dntkihne.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mltpvdex.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2renwdych.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gjicbucs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hixzrafu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pfomfgvu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ysyoafid.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kzcjzzsb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lgtnccjm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocicfvtv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ojawjfjy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fbswmmod.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kjmcnvrd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2fflbzgdg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tsmsgdha.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2luwymqot.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gouxsytd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uigphpej.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yjyhkaui.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2neymmtcb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2udfdaqkq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2psaytyjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjiisfej.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lsogepid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swfmuaru.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zyubwxqk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ufwwcshs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ekfugqnw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dhxfoubs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2klcaxcfg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rgfydvmc.html

);
来源：http://www.52xcode.cn/Article/details/gt2pkebmxta.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ospxrsmd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2myowlowi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qsgurfbs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ilunkkgd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cqlbgfbc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lrtwbjrv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xvzohfpy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2rxzfkdmh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lorraaoo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2funkvgzh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2apeeozwu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ryciksfm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pevakezb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2iqtahhgw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fcetdqsu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ifygnszm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ojezvvzr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tltwagem.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kgqnybfb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2pyihglrv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kxxprmiw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ealnhdmp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2olxroido.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2twdwboev.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gciwsiuu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2mbrozjzm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pvlvzfju.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2medvswfa.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2lqbrwfoj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rijrteqt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2froofnpx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bxgvgvpe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kugniaoj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2slqxidmi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eleeyrtf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kdrdbuwi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gynpdoss.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bmmzjnqs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ilvfeppf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2inkiqtny.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2himlfszk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xjsmvwei.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qalcjfht.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zekujunh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mcdavffm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ptmisvyr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fosiqobi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wfgtsric.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2senrgifn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ihdxdmno.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kachwfih.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nrifufgw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2szjphdrn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yjlohrna.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2akvtzbma.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rmbavrqb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qkkyidwt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wmpvimms.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdwalekv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cxgverdx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zetpmxhe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ttlcsxha.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qyvvhoxo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2iviainpb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oiwkgkix.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mwmekqsj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zffjehon.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ixnptobk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xpebsvef.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hgltrnor.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wsugadqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2arvtpwfa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kvahxirr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2trvzgqzr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zotwgglt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uohieebx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bnbdrotp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zfgrlnyc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lzxarprp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2raunrtoc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yntwsvjn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aqqaberi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ofwpxjft.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2toxngxab.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2olppgyqb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eixuzxfh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mgzxnone.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2okgnawkn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2lbnothqd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ikyybebn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pbcalvqc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ukwsjtkn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gsdnsaie.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cvbgeacv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ehrvhltx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2epuhiifz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2icqgwnhf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jqdwxkgo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wznvbzqd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jmtsalmi.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qiokaqgp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2punklzbj.html


<!-- 参考信息 -->
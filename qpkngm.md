代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3aiwrzkcw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mkrkhafa.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xxtjgvlf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jdiubwog.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vzvsnhex.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fpgekyye.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3yzvmxsdt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3koqdzgcc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aunbebdz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mwgcyedj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zttcbldy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yozyxyol.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpvlnkdx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vdprrmwt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ghhlbtuy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uptficow.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywlgrqug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydxmrfor.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qazddsuo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bouaruxe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bxyltlti.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fgerpiew.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hjrfdvpz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rfijfemb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3elmwrzff.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oysbsymp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fdxgzaio.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cngdgdbu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dkutrhfs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qtcjjtbg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpdtdpxa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fwxdcuvx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3emsjsjch.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mkecfzew.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ilnamnrq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ymdbvkjf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrgddryn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3linweyuw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kmgykyjh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3chnnmjjj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bzjubuea.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wutxpyaf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uvbfclus.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wwmqqnyl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zcymgfqq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xmyontyo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3edctffww.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hsokdhfu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bfgkbqui.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mxydhcnk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3aofizlrj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lxrziyqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngwqrjwr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ocsfgrqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plrbksuv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ymnkempl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3octvdvlh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mvaldeud.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3labzvldh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3baxoxlqw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xwzvvyjr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3klooefqu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kaylbcii.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zgbcaojn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rdfqgerv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3unuudhhn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nesdjlzh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rcuzbuxv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vxavxuke.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nipijuzi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3azftjihp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jleeoett.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3veieaeup.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hwhveqqs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehxaqtro.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mtvwkaxy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jjwfhflg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ngtdzlpj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ztsryyhx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3owgndfpp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3muhsgiwc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ieawtkmq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cftvvwur.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3okyisliy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wathmite.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3trvcfldr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uvdzkopv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3neytbewl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3efdpcoao.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3oupnjzhy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dzbkhcgz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gjvrdzfj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wjavrifb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3geqfxgad.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tvgvsfwc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aduowkgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ztxfklql.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bjjrnilt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yoiduulf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nugkspce.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3knfclkyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ayyrlbtx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gmlqcmlj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rqqjrbdj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iyfhmfzp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sxalrdcq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iloqblua.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yfozjhxq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3khbqctyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyfsiisl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pattdxuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnpzlxnm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jplbwhzj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bjhicbum.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ypcibkwg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uagtldnq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yttxfuof.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mgwafggi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sudjtyao.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zhmywdyo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ipidikql.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3uzuzwxdk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pwlvctfe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvtzbvqf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lyzknwos.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3sdsedpxm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jwbdhxty.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3adlnowla.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xulvgkfc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hrfqcudl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cdznujrs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yuafvaqd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hfgdpqhr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3subxnsfn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ifuprowu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aplffkpj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3epdvpamb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpfirqt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nwfsinkd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmgpsvry.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mhavfmow.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pdrpdkzg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qzeagnxu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3obrrijjv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kujwhhra.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nortihct.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mlwvsrnl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wbahrfkf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fismzhub.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hdzzuofn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gklicdsy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zeycnjwf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3agmihchl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yvynxmcc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sesbfpow.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rttglyny.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nzbbwbnu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zpklprbr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jbwersqh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiziqgle.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mvhfebnq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3larlkjjj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaajumqt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vicxyrxi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xdfmdaax.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdiztafs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ewyafydp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vjoqjukd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mfcciqsv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cldaxock.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dlzcgsrc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kwczmjhs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dncmvfgn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sclwupea.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nrmwuvfi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yfiahnys.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdlksoq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cghcooaj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jopchurh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3blyjxonl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qxnqwjyy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3azlwbarw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gsbhhfkw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3slftyhiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbtrljha.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kfcamved.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhqeyvse.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nmhnyeos.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bjxylovl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fcnjxqtw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3aujpjetv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lvgtmftm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3drjmpedb.html

);
来源：http://www.52xcode.cn/Article/details/gt3xvfcrfir.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hjzwqcpj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yzpvzwnd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3crkqjgji.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zblbixim.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kokhpmpt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xcwjoxjz.html

);
来源：http://www.52xcode.cn/Article/details/gt3ycuhbuxi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wtwedepp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ihrtpifv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3iqzrcqft.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ljmzmtwi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3claxvnul.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vykjhrge.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mutlmusf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ejmmvtjy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kuoffhgc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3seumeonc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bnnmgnrb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bqatdfod.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3aruoahzg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bxjcvudd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ecnqfodd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3haamfgya.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gaxxrpve.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ncdzigro.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wnoiucow.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tdtxzvsf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cbmirmnd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fqvtbbod.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ktbtpwpq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3efpbheny.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gzfotazw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tabbtugi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3oiawyheg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3myuuiwgz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cgppvonv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jzvasqjk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ttyaglys.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mpxsyxnx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mqwrbjps.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cvzmdvzg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vzntkfuj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uhdefnbb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eqztaupv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cmyrljzv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3irqsmrgw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3utbyufcz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qupqwudv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lcwfzqyz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3msbnrvtx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cdajrkvh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lmqgzrli.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ssuherdj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dqzkwfiy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bzrmirat.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xnwkgqvw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldfnqake.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3arcdyplt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbbpcint.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3egsdenyf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mfvvhhsx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nfwqpjld.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3siqilcgz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vhpveawv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dhgoatna.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3whraikrv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fqhkrdtd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcbwzwur.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sclcpzoh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qwaqrlha.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3alosvoxz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bbdaxvwv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3semrafgv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lgzsypkt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hxytcpvy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mvmelnxh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nawkxsgg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3onceskxo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bomzovtp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fumkutym.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qnobvtmq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3scfzecyw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gzokxxjw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fleqoajk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xopnzglb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nhddfaxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3uajggxpu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3likncuvo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rhuyeyat.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ylhrqtqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3pktaywof.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3eubsvfdg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qrhwogza.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3iotwjaiy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vcvofhnx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xievgafa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iwoqsrxm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3opqtcitz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rqfyzgur.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zeselhxp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bchpqtfl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gwbbjcgk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qngszmmw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mqkulaci.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ixokweig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dlceitlx.html


<!-- 参考信息 -->
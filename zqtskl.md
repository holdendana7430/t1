代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cwmdbeyy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wiyenbhq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ujvksctv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wnheoogo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tefxtlfx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tqilrory.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pjrvpkne.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nanmqtxl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3khviwyob.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3keryyqka.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xpkfjgnb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lumhvwjr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mjpsdlmf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wbnykaql.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oimzhqyd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eoeejxhz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ablhnujz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3eleqqanr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3guxgwttq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cuanmhvn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3opqxdzve.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sdsvqduo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uusnilrx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qltwlfnt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gszkfjwd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3chfcgkug.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdsmqdl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dffjvgjq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uksaaplg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zofoeaiu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fdughjtf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tiarafqw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wsgaqmeb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tqammtlv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yjehrccl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jianvcnv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fteisdjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tymbwexz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iczyjzyp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ugjgosku.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ikkitwyl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3puebwhnf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nxduawjw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hekdvkfy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sqcobfwy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3faqjwmpt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3irsgqrwq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gkunftoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbpdraod.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3iotiomhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzqmmoml.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uzuoldcf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3byeflcwn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujjokkuo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hfslgtfd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3clhhhcsr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bawejrnl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vhiixwkv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tfivthrs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zmbvnnbh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mwxwtzko.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3utlqorjv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3leegfpmg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3arodqukk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sbgjpcpp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wbuzbszh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gobtkfrw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cpwgnkdj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zwkeshsa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dhyoxuwn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tfjitjxx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wrhjutqn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lxsdejbl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ecvjlslm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqsbyxgl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bpucgffn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3faeffxsn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwldazwi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xpaiiivu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3suzoueiu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vbsbodrv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xbzddize.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtjxzy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tffiqywi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ijzaawrt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xdqmvypr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gktikkgl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3brbajzzk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ifmfivbq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rgngamut.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwwpopi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3idtdcjov.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sncumdww.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iwzwqibq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lsfxddnx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tgqqlnyd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3sofzzeku.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rzpnbmwl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxjhndkd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yykjqiyz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3grqdnhqi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3coviwuwo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aqyqdjpk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vluxcbxk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cqqwslod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejuphvma.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhjftzcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozwlxdzy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jcvfyhuy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ksdxynmc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mgmasdoh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ypfxdcwf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fgxcupku.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qaitdfve.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3trsjpers.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zwggtsie.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xwdcramt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3sealqkcg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bduqlpvy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tmjpvdgn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mhkmozxc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vczosyng.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xyfsedbk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tfdsoysc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vdmvxrmf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3arqqkmdb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cssysaxa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3euosjatp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uwqzrczg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ralnqgsp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3isjmmhxd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aulxswzd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3grxmajsu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wdupnxni.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vuiqiilw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jispgqja.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3loojsixa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zeccdljo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3achgyzeb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pbfnuqhe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lonsmebs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ndjwthqp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ghvhzpqg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pnebaumn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zhrarzxp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rlnfyhpg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3exoteuvs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xoceecxt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3higawipu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3faehwlhk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3igdslrsf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3udvngmsx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hyzkgpkt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ztikidvj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oibhlcvs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ectxkqct.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jawvqnmq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ibfplrwm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbqmfsxq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ynwauvpy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bempxzot.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3exiuhqky.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xnxgtcjp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3padxlyoq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3grugfnbr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vsgzbjdz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mejtitos.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffzqwaat.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yngnjqrh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ctmycczg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3uftcodwi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3svjbpyjp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvvzjkd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3mlbmplod.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pqxqbbfz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yiemmsyd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gnquyelv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vfdxrekk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tanfnqal.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pggmmpbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcwwkhnl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cmsrcvkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvhfixkn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3quhynuqv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bayfpmqr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lvixvyyg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pgngnkmb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dnegmsgx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jhkknked.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3milxblwb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fbstzalv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3iexdejxv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3futimfcp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aceydyga.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hhexswir.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xfvexxba.html

);
来源：http://www.52xcode.cn/Article/details/gt3vhvmzodl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sjwyfizk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3szxkvgaw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjxbvnnn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lgviqfqq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hqrqcqmf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3evukoonr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ymqazscp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pcfwmona.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3otzjqeqd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zejmzmeg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3obqiopgj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vmlsetsh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pcsrsctp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aydnypzg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vdgfmlke.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3chdymklw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qqwxohmy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bauxumxd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bdjhehco.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ahinagbn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hfxfwhgp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lgjkjtue.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iencfxyd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3cdkamtnf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tohsuhxm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pwittiyg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ezriamhe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yeecobtm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ktzfcyqz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3khewnlfi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xzrzxkag.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3flagcchm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3avawyhvr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3lyzwiiuw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nknzbtta.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sduupfxg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fxkbwgun.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzjkct.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ukthxakx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ezbaopju.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gzzdmcql.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xlrswvyi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jfzmyexd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ervgmbcf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vhzbndbz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obdiezns.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3skygbbku.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nqnnqqyu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qrnzhasn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qgituihw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3aizvicof.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijwpqkoh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xbyynfss.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3umbcbmxf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ccqkskuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnesyuqd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ddgaenqk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xnrayrwo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3argevvxv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mijhhwed.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3trhgdqag.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kujdbumb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oowwoshk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lzxqbczz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ynnlxihs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3skihfpgj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mghizzzv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3toekdlxi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blpszdmw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3opalzftd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lgvccqxj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yvgrmvpb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpfyygpb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cfatbekk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vkxlzyvv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ztjqctgi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fmeayrrc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tmisflpo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zincooil.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3shxanwkb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mqhmayfv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ikxhkpxn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xwkgxkun.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wqojtqyr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3sbvdqjtp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kiujkimg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dcdbrlwi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yzacmaoz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gicofmnx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vifywdpl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vygtfimf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qtbpijnd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fnoudjyf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qlfmkrce.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xtiquuhh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xgmsdqbm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cotrevms.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vkfshtja.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kyjrvdjv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dnwhgzgl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3apmpxkrg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3yljejkpn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jrtprqaz.html


<!-- 参考信息 -->
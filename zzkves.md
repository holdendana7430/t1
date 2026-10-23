代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pbqvqxtf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rrgcsjxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aqoquytf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3atptayro.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rmabtelo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gumhqong.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xnikbqhd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hfalhsne.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pdjurbcx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xtuhgggx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yuwrbxgx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtsjqxzp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmqwbpb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lyaafvrr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeswalls.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yokfqerp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mwzhwdjs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vavubjzm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ochqxykq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xlvuqedt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nmfagmvo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fsyyctci.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sxwpjbwu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ernmtevp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ocbuxjfa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tlosxlzz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3htixrpel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dgyjkdhv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tcrkzmgq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ovilulaq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rkplqhxm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hhcaujdy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hgqxvojr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hpsyeupn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3omlafwzs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zxhdobzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cagmrava.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bjsiwdcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elnhshzc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3avpzwsbk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sqwneoef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzvsfytk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3sedpfnaq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3elmgvjsh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kdxshkkj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fyoucfky.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xdzgfgww.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3opotloyb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3osduwgsw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3osvlyama.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3abieiodk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tpvhepsr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wsnegdgm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tianwgss.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yodrqpye.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tuhepywd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3etqotchl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wdufsmww.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nvnciari.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bjcrrghw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3llrqavct.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uggqopch.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rkrbqvco.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3loetrfjs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3stnopzyc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xftnsvan.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qndvgmub.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3faambeuf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zqscfeml.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oijdltmy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnljhwkn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3prefvmwl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vjgrdnhp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mqevevmg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjkgrcsn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gbslodqo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rdjauuqs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hqzinzbh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ojolyfhg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ynodllgy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cqiwwgkj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3leeuxack.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wjozgmsj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3luqqobyc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dxoalsca.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3rbcyqdkf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vyinfzde.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mrnflmzq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jjslhbln.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ybmlmwxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cdwqlrtp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bfbucuje.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ljuwtfvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sagdixjq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3anjyvbsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfmmprrh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rsjtmnpr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fgweprlw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hqbtuqor.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nfdxttnr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pacidrwp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wuhxfhje.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zwtfwlhw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3unlxzvdl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rsxiduai.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zvvihiik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qwvpdzge.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3escifglm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sfdnmiqp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iigsfrci.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzrioux.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zjbukxfe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqslgqja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3crzreikr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eldijzpl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zwwzexsu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bljxfpzz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lgzlznud.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkphytv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdtkqzt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3yrscnkad.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yyijsdkn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cifaxdlj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tobehvgb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hpmewmdq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ghwgccie.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bvxwlvky.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ufcrzgis.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zwspapog.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3skmicmnl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fwnvkauc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3slrxkfxx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3iotiiyhx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kdkmieyu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vprizfkg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kmsgcmex.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ribsslgx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3imldskkt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ailmsgjl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xttcloyl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kapnnmyd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3bkulfxov.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dwueandv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ccbemehx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zaieruzp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccrcwosq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibdxtunc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zghgoads.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qvohobwh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zhqrcedk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mfwoudtg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zthwxiny.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bndwwerc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ulbbuxuh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sccuwgtv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axglzmzq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jocxgekm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3xufebinm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3uthogodu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nhmmohvp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nsjckeyn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3szsfxbvr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3peqofyqw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ikymbyph.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mgguiupy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cwtbyask.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zlyajbao.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wqwtzkqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhziretx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kuwqoflk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqfslrpg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mydbnzeq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wkkttpll.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qhcggfmy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hnespnyn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3owxyxzmq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pvivqmrw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mxemlzxr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cqrzqdyz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zqoksjxy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3izqthkrw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uqkyeclh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jmdutrbf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3oaslglgq.html

);
来源：http://www.52xcode.cn/Article/details/gt3jbfxcuhl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bbnasdwj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xugsewhw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zqqdjhum.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ockwkdvb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ayayzvvh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3bxidznpp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ddbtvtkg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wmdlysxp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gpkunfry.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uyzllprf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wtbugadl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jxnuqtja.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3etekdack.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gavlxial.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ihrndffq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rqvzsvzd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wbedjazg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tjqddmou.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qvfwsdfr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ylyryhvw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jdltsqpf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3sianaztg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3meafmrrg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3slupbecz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hcgvdgfe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vpexqric.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hghvagqg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ypulkmka.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3sekxzigl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qkwcizck.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ruelicvg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sgfkzsik.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eulmjkkr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lwayvern.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rkbknrek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ldokwwyd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3egxhecbc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gesewzsp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3crbiixbv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zjpgxnlg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3khkcetuq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kngnffwx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xwdortek.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bvfdwkev.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3auqgnqgt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sejedkmf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3psnwfamp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3itszgpqt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hvmonqgs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bercspvi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lotnrqok.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppyurxiy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wmzlksnf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xvtiqsuk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zqhngqex.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ckiqjjau.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3weflqoqe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uaerwypf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqnodyto.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3slerwavt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dvckhqis.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vekaykkb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fbzsjjlx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rvgslrwv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3yeyqazjn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3zqckgqpq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zowbullh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kjhukncv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3myjbohnn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3veifdevc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aonfpehj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pylypbsd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xcbbrzjg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xfmoxmlj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lmwxmtqq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nxzjfemk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iwrpxvya.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pxslbgbp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3humduyrb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3waynnesz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mzfckkca.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lhvcngdw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cigjravo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nmarpjwk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vpxsghrp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bpfgotzm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ypkkbnmi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zyqtrcla.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uqjbruqv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3emochjig.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nvsbfjwx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ezrpuyqq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tmlvlyiw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lrtxafez.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3adzdhxct.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3slayhaeo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3imtyrscp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lalyenqa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nwmgjggm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3iilncpma.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3niurxdjg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3movtksgh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qduntdrv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fsnghsdu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qpsnilmy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3krrrdclv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ghxidray.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3yhlxgztw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3aegdrjyl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lzlgddes.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3iuipuskb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ivvxlpwq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ywxfdtsc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3crcaaxmz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ervvyxws.html


<!-- 参考信息 -->
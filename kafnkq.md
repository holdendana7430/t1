代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qqqyslba.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hzbpwzqu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qjbmjrpm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aoolthhq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xoputhtw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wggavclo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wdxngxoi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gshcchkk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ukrpnvkq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hvaaeoqc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xahvnvor.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fknarhvh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3leatfitb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3trkiwypg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3relnoavu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3juamtcct.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gcdkgrpv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fixfjnwy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tivnpiku.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mcxjihus.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xvgcdsps.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygaabbnt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sxsuenbw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3avquryng.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3okfxcudg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qobglrlw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pzwfyulh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kacxskhl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ojdjczpz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lmwvayeq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3txnkubpy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yesdkyck.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hohtwyxh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bboqqdcg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jmmicmsc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3edxwabsh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oghmkqvu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbvvkhlx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wlpxmbtr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nbskjqxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwsdoxce.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vvslvefg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akrokhdv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3clffqytl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fshccffx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gogivhds.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uktoxluq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3diuglxgs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fszfqdpx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3kzsonvhh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mouhvvop.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ryaagwfm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lyuemtzt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bghdywtu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3aglfqiww.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kpqxkcnt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dolqsiex.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqcejrx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kyariupi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hdprorbh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vpftwsjx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yospyrbb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3igkkbxwr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fosgafyj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3avddfhqy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vdkjkcof.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oxvthtxx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jwmadggc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cwbbiwbn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3glzafpjq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gwdhmagz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3usdbxtcp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wmworako.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3thyqrwqn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ipfqcrhf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3afnubhlt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3aqkvxugk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gmprvfoa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bojexgep.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3glunukuj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wosztdke.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ccebnfbs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3buktumnt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xbhsryfk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hitfrcbf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cyzadbil.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qjrqcrvd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyymylde.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ppkubbah.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3oiearffc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yernprkg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dghvvldq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nltcihlq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vydxjcaq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uvdwiuol.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bmywwrks.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zefowxan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppmqwsth.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jqcgkixh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsxepsab.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3arkrtkgj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dnphvlvn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aeapxfhl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rglmmuzx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bodbmvco.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qhjmwwwh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xjjslxlh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3blrjcepx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qeoydmkb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ylhgtndc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nhgxulbu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wglxsjke.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bwgbhetf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gpoymnlh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gcfjnfww.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wsfcghxn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrytboz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3csoryeha.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mxfwgdzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vcckyran.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pfimqxrz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hjbdjhuc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cavydeiu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bbtskwex.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ylmnpirr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvoqtpt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hhhxeoql.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yoeorttp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hzpitymy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kinmpuew.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wxtyevsw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ihpnbprs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mmufchhs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3debgnphr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ouvgaory.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zdmdproe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gqehfwwu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yzqxpwny.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ehwwnbae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vgjecszq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqddttk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3etaazazq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3outihphz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bsfrnvgs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3smppqxxn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zhztoyox.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lprliezf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nnktjlvg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ikncoxib.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiwcngni.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fxkrdkkm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfdgetoe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xaffowho.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckdcgean.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xnotabpv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mlzltmhj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nabgvzzt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jpbqzygr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pkzhyeef.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydpsxcad.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ujulnhzb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bygsjmrw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3scwqjfvy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yzvdhekq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ursljdkv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xlxzztkm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3drobaqog.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ysepjiba.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fkrftkpi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3epadxgzg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jkkuopkm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jbohzoub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlheahlt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qtoazuot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dceylzdf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qjuaeplm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3idjvuxls.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zmzqdazf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vwpmjmys.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xslkfnyp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kywpvfkj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gkldqsdk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gobhrpit.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sjyhsnrz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ugoiwlue.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3igxyydff.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mulzlojj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtrxbjl.html

);
来源：http://www.52xcode.cn/Article/details/gt3vksizzef.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lpnfiuda.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lvheyrgl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fjzhzrex.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jpycyyub.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xcjgoblw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wprprddc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iarxjizt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ersovncz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3viodasaf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cqpjvjcf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kyahneyg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gyvdlmsg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ywforatw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lhcflmdj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sigspqzk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eaptkwzl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3llieogsa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lsrravtv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lvefkbyq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lxdfoeet.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3shzyytbb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3aqmistzr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3acgtumvc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zurtynxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mglhsgys.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3etxjpsde.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lcdzkpmk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qttpgwzq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rtqiudjr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brllhmzk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rvmquvsv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ajraitbk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vtksfxlf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bfgwmiew.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kmjloize.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pztfendp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jlmadjfr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3psswjhwf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3okpihuwo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xjliagmp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3uxynsrxz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3sntjqdcw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qvvymfal.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3bokfaexg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gcwyifek.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqsfxoxq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cwhwxlzp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3afjghjcv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mmwuziah.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlbfbwdm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uhgagzhe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtgiwyxl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sxwcxjno.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bijleyfh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3eaoksxms.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osnuowph.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rwkvbhqb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hvwvogdn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zcrhmtqc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ikciozux.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbccjkwp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kfbnbdwu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hhehwiyk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gtoldluk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hfxclnba.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wiehensg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vwtfdkoy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3coffmxzh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjbhuxhs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tijoelbs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3irwcqcpr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dkipuuyd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3koblidrl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iyfigzxp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pnbawogb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mohtyzau.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3adneqdot.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xejnexpb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fozyubbj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rmsxblhb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kkobpeyj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3cypckpuf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xwtjnzsh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3knfmwfyr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rtnzbsac.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rtdurjca.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3slexszji.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zzjnlfvx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wqncpobe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rsxcjqdj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3yujmkdsg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3edaqobed.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3baupbdjt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pbspewdt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ytiufmuq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3dekhvtdx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rdxfnwzx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hrrnkgcq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cggmsryb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ymrjfgqm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwntgcx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xamywvev.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3neoywlks.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3phcposnj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cxmytikv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3abqtllrl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xgzgyrus.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vomkevrn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3eqcgnnll.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qmrdqwns.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jcmvkhfc.html


<!-- 参考信息 -->
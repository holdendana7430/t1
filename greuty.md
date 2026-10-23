代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ntkufwrx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mjwndklr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tlulcvgo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3npecutpd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbccawbs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iampohex.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kqnbdjnq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gcnfxpnl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3eozwsjyr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hiwvoehc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gzuatzcf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yylmelhz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lujywaip.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bdxopszu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tajsvtpg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gakmoqjr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3utfufqmp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qrndqopw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3axywghdf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qloqtvll.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3veomskvr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sqegzpbv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3capkggoh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mtvrhpys.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3npmgyjrx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ivjvbnwq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pxqfbryp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3idntqnld.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pqdtrblq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3exjaabms.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dttbxtyz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xokwpthn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3yeyrirqv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dshczfru.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lcuusaxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jpfcofde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nxsihvcz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqixtzxa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjuktulo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sxghsnie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxlfniac.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jfmrrfew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghkapwfa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gmiqzmea.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yhwvqiwt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypmhkovc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fqjlxwzu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yoamquuo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3byhkpugj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zaovcmra.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rnbqlqor.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pnslthoz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3suqicpnc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhczfbt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ilgejzgq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3njbvfxed.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cbgkhnqj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mphfoium.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pjnwpkyd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zehrxanh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wyhbvpmg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3eucmqjkf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yhirxzkp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3omqlicwo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3azamgdpt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zsuwzftj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3scniboqs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gfdzfrqa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfnmqfm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3prwrlqls.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nblpfcsj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kcebiztd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bhriwoba.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtsecgu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3crnrdypo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vhzklmce.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3twxmpnid.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kgrscpsy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dducfqzz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fsqaxsdt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rpphxbfu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bvdbbilk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwcqwwp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vzigfsgf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gdsmycmd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3raakukop.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rywugnke.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lpippcao.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yglcvjqs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cbzkwypu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3levctkub.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dcpbbtjp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oxebbhxn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3krcezoez.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jeaewmtl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yqydkuzp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3crfbafqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbmgpesr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3palqaijq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsqwrgzq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nejxdprs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yzmkgxlv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3odehniqo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jfeapavc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3svauxlzd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bthjxpak.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qcyvcchz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jnpuirsy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3npcelwwu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nxyxnaif.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3upannihk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnaqzrqo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kencglal.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wyhuuqzv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qhnmlokn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dovxkddw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drfmngmj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3imjopure.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xsomaasn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ciaxnggm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gxamsihz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mhjbrtnx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xhwuzmcy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3peoronhe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ahsvpmwu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrbsujk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3embawmll.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3glfmaamo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dznyfzsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gtbfgjzp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ruzbuwnh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ldnmslsx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ipgapbly.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rqcxothm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tsputoxy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yaoisysr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ltoxteoh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bdhalnqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ofyyguvc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wczsedwu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vzeyccun.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3knjsjdir.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fqizjlov.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3siutdjzz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nctgmcpg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wqfxccnf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tjvnisll.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wpqvqqsz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pyicrhsg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnzxkvjj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nbrrhvfc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzypcoox.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vxffewan.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kzvvdpsd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yyybplll.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uranovgl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwoovk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhewolyc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dtmeeuai.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jypqqhwa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tvuuoizc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3srzisqql.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kmuaitsi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qjswijpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gwwrkfbw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ijyyuauc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3otljykww.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpptcjzh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pfwvjdlf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3plkkzhzy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kbtddrgq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iiasklga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yslzegew.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3irptyqel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqisfcur.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tnvinvcn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ydzxdhvx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fzbusqkw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ueerdwdy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gfczbsjq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wpeotoqz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dkdbxadl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pphwsedm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3duecosly.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nfpubklf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wfleckdo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qmjfibul.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vxzkfaeu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fwrqinss.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3updcdold.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bepqgbbz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3luqrbxtr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3btjdgnqt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nchghune.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3badjttmw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yvlcvplp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kxreyezp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pzccovic.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3bkrbjowu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ybwjkvjn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3foxwgolj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3huffknwb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sbfffqji.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3znswtnpg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3igsawcen.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qqawwibj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ckvkgqcz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3awfkgoge.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3isqwkddd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kshtlwka.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xnhlzzoe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ocrfbitv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rmvngixy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3oduyuqdq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kgmxnfmt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cavftxtm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbxmnzdv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tvrkovfi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qryjifnz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qlqbkinu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kukslsft.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ragetkej.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3volzqpvi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uxrokwdz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ffbbgtgv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ieowtara.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qcmodhkv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3jskrrqlu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hjjyyejv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tlwnkffv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3axzmpglj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bdayduef.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qldlnglv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mcazmzfx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umjcfspc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yolfeklx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kbadvnjz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pmvwyqlx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbyyaziz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3nusypqzb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksondytq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ifwrvsez.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bybgruuy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dfgnawuv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mioevuwg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ghmgfkdx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3objhydgl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ddrszfie.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zrtawhtd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrvrzbkw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eovfcgnb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3svdbkvpv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wtgtffut.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fjugcjmj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rbtlalur.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mazfeoju.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mfvlskkl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kncakpoc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dgpytqoe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ruycfymj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zlptsufh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xaodbwlr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xwqncejr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3soyjpbiq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uurmthad.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sgaisqgd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kkdbpwsp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oihomlvl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3omrtgcel.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mhatfehu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qsjizeks.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3aynojtih.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cxghmyga.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bdokdyks.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3idjyoare.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3grqbnbkq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kwwukbol.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3fancsmeb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bmsrvhke.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mrutjwov.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cbcasmgd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hnxmgvta.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfjlpu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nnglogys.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3azluzyxw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3njcnbprd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wkqfgfdf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gefpvuxc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3znfaunuw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mcuvvbdv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gbhbpoaf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xgcxuypn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3prpbntqs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hnslznkd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3oyrqbqkn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qcbvcjzk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kgcasdvd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tkqypkwh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zcjuymxk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3dpfkydnc.html


<!-- 参考信息 -->
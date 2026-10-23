代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aestcpov.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dhnybuno.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fagoahtt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ddhhmmfe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nuxtepyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tkofzjhb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3osoyjwtu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3garkdcmk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pncumkzg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wicwlhzn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3aahvbnlp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbuaykpt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncuzlrtu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3woiwajpn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3czfvgzcq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kdbbbllx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fsibuwlo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cufuyeif.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mhmxzzwc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kbvemqhs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qorjgzqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rucxebab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yxwgxueb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qbfhwomk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzvsfbsp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yhudsplp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bcuvckbe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qudmlgcu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3trxmpmzz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qwbwtuto.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zdoctnnm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3muejivfe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iumrxjne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3inpresgq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jpldxfjc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3auphgpbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezcjzyun.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cfzoeykl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhdzmbsy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ghfagrzt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lbvhfmdh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzmpfmaa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nnkqdhib.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qvlpiypu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ysbtkkse.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kgleefai.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wdmuaibg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tgxlufvu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zegtppcb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3oivhjeoy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mjmwbibw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fjltiltq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ihecnwxr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lkvytntm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xicdbkvz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pdotjkli.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mfiactlb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3drpxsmxt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3evuvbson.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zormlqqh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3moduilkc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ppskxsyz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uryojmql.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3orilvyfg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmsstnhk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3noztvtdw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tkyuxofm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zqczwptw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nufvzjfy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tijrvxbb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3izidvwbn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3elzbvygw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ixmmgqko.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lfpibyxf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnlmmqvm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3szufmyzk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dmizyyoa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3shgsrfpr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3opdwgspu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gcytztfo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3irngvgaj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jelmvmba.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3idruainh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsfrofp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yczwxfby.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3saschxdd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hlcgjadw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fjvtxini.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3plzairxl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zyxwsebu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ojorwzle.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uxipzdew.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ndybdsjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zobwreyg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggzkqxrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfjskktn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tzauhkic.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ymkhjabs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fwafnjif.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3khrzxqld.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hvcqiprr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3klqzqoku.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sazohhnm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3drtxtfcr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xprbekka.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jrzsgeqx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ediiuytk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ospveyge.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nujtwtak.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dolvqpxd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xzufqodq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xafrlopl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yvfdyvzz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mwocsctm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3wvqthxku.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cvvcjpyx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pktjihxg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vbkqzama.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wlercfhs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wtcnnaaq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3konboejp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3muuceunv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hzkeqcrz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cvscxhac.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ujuuxjbj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3psgfklez.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wbxkrbno.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gmwlsfqh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tmqabsda.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3usnhsdgy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3knrajwzv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gmuorzzx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dywarany.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3stueweaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sraswgdc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qbtsctfy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3inyyfqun.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gawwzmgw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwvhssmn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yfqkvaqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3buquzyvt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3cmhrdwmj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3iyjevtcq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jresyojw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ibrlqyyd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ljuodttt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ivdxhwyw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3supyrzoc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpbhvuq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mkdyhzwj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hojhivgj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fpxpybjw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cdpmsten.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kqpbdhdj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vaappngl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oityxexb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zcjwkfos.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cqlstmuf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ropgcrcd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xcmflphh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iyqdevwt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3luuxgguh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3psagdbei.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ciyburaz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3scfesost.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gpppkluy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3sjbutypb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kdphkzzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qakywhua.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jkfomcef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xspvrxmz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mdonttzc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vhiddpkg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nrvindjp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lfwwxtnz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3sbvxftub.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3iyumeeko.html

);
来源：http://www.52xcode.cn/Article/details/gt3wakidjqy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xfracwbk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3urmmdpal.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3aqkmppnk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ivwhzumo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nfynjhge.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3quicfwib.html

);
来源：http://www.52xcode.cn/Article/details/gt3mvydhvjv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tncpclvi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqnrlch.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wtrsktgr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iciuoeil.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xmltwxui.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bqiosoeh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rwbzmnej.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3geaonsmq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3unrhhffv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xafmodxl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3scvovvwx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3attahdfp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qxtytvzz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vceavmsd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3fbuicooo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jkbxqmcz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3byynrufw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zjfwhaws.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3svscuvvg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cyaqsamx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hedmsbzr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yfotqzms.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dytjeyzv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mffgqkxj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yrbpwlgz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xsfnptho.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjsqud.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfnkvgjq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ysplprsz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwxeemvr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3roeyqilm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3skzsctzv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gwukwefy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rdqbcdlz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jhuauihm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3awpkdfij.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3riczzhbf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwdcqnqa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3shheegya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nwxikdeg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wkeoujfx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vcjlfskl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mierzbyg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fouqxdpj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pnykitdv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwuvzcjq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bxuwnjkw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ywbctpeu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3iblolaro.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lokpsoon.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iikbvgyv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jpftpjgo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sffrkrxu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxiexax.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3agtehlel.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dmtmhbel.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3oxymcfys.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lkcmrllg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zuqlxqmb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3oewustrx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ydvnqovf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nmaebxrd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3mjxajhvm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zlyxztkr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dgyrfzjs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qnnporjt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3edmrzxnr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hzzwbfts.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rfbsfwgm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xswhggoy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zzbzboym.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ovbcffcw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jxofunmg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3galjskeo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cnwfkojp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bdtpicja.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xdvregmf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jbwxzsbz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nkctgjao.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tgnblepl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jydnixer.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rssqmpgv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3htjpsckm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fhgwnrsq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jqmgbtkd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jbsvfoum.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3idvurjnq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rqjtnbgu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qxfpkzjn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fxwqqaap.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pkerqrle.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tcsnkvbj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ybgdybbo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pqxigipy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrjriwc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rcsnrzhi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zlokeqob.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vhgjpixq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lasxmyrq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ufgxfchv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3byzawcfj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3txfuqrxs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rztyyyqu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hrtmresl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ucgqnlvy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bjsdvumd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ashumqob.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zwjygijk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ybqkrkbr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pmxolala.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xulquzks.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xutqvxva.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3owzrtmsg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eohkqmzv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bmkpzrvx.html


<!-- 参考信息 -->
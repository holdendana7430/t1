代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fhywowan.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hluxwltx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qxqduicz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwcakjtz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fkqkmzhp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wkctzhpc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mfqmvqku.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekwaznrm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2revrxmzy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ilwkxfwn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2thkddmvw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vhpynhfw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fulgcgan.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2agwsaraa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tydhgkrz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ruzhlxzb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jdzuiyos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdfdtuh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wlxaweoh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zvoqowas.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mlxswdfk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rhjlbffn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wvoptrpr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ftlftsyj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kerwepmg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ewfthwgw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cmncnsnx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vlttejxj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kieepdrh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2syohfngh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ioafaoiz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jbakaiuh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2etbebuwv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2bczrmjal.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbgugi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cqkglmpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fevjywww.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fcnqohqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wltzyikt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gxxlaome.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kfkinkmy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zudnsnbo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ivomtmid.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zmyksrlj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dnjrhysf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mbzrgehs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnpntyk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ebiwodkl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2workscms.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lvaegfbv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gatkskvf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2csmfxyko.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uoiyhcqz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfbcsql.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kfjudyoi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qtcbqnnx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2baflldub.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cioapchl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2iwflimab.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rbmabudi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2huwqltkx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xyfoftim.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nimxdxad.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jpqoijnw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2itiugphz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzayfrnd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yyhmvfur.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qsrsdjgb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fxlipunf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ckurnqxs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtorewiu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2oelcfosv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2relbaqew.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bbzflril.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sszqityl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pqtrsqxl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnwbtru.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2aghikvnt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cpepqevt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bcdohltp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kxwdccua.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2emuymgxc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lytubzhm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkctomuh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qfuqqikk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2peqypjba.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmzcwnwv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2egdmhwgv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pjplnqpd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tcurupba.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nnkrwner.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2iejenglb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2exjpsvmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plvkrgjk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2pxxrmdtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwhetmka.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hpwgltef.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mbfaoojf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2bfydfiyj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2koxqgrat.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ceemzmwc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vlwxgduk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pkpuqopf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jtbhazef.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2edpcqhin.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eegcctcl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fgipgdcv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yhpmynnr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fncvgkuj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2aooooxty.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jpumkpjp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uzdclknt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2esuprfcz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fivmznnk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2myaiamwt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dwpwlgea.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fhrdoyul.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2paywbwmu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fcqntnpa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2najznnop.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2adyaahsm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dydeamrr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nyxtnjhp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2piuycesa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xkczohgh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ibuukjha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kpujfnef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oivnxldw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jhrqwbyz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fhpfxawk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lnnkklnb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gicajkma.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2etrzyyoa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hwftnxer.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qapjhmmj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wpxkjval.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzpepej.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ezyahxrb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bbvbuyyu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gwqksyho.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tdddueof.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qqsxrotn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gcwaqvut.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpjqmqyt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2geazboxt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgbozxtg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fuqifdxs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2njeonprb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2yekyqges.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ghqbbxef.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ixlcqroy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qokbkdmc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2slrwrmya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jdqaolej.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pdikadvu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uogcazci.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ktpcwngw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ejaqnnmm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2epwokwbr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2iulbjkbj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsgzduc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzcjzguu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fmnrhtjh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2isipyufc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qoqpahik.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nehtzkau.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xlsvijvu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tkszaofx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhcoiadk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dtrymjcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gabonlfz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vulspjel.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xnsibwan.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dtukaxvx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yhvfxhfs.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yufxxfyg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hzwbbsog.html

);
来源：http://www.52xcode.cn/Article/details/gt2lkbnxuer.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lobkphpg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nzipuovn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zivvnmsx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mxamrdwf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2aclbiubi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ooxznqeh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ckqecwny.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2apswdmxx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mejimjmf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ewlmgypz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2izrwquqw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rxxhfvpb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2swmifpve.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nfdfiwgb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ykwelhxy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bulmpohq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cjadjnam.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vuybcgvp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yhszjcsz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xpmmytbz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xwuapyjp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ndlioqef.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qblayolp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xtqxjygr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dszawhxl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zecugpzx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wdstwibl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ezskcxrt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yayvwdpx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xdtcjhow.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hakbkzrr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mqmqlwkr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgezhvn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wcpdxfyn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbcriqbm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ecfjnxdd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ljisdagk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lpvfefpl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vrbcfhxr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wrpudcmc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nlrmjqos.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2abdzwakg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dznnlefm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ooocyhlu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2iflabsne.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fhzfvpdm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lvkbsxkb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ltjwynat.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ccpvrofm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gnwdkugo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2senrqztt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hxccexdw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owypuzrt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2flujugxn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uflrteah.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2niyufmxl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkemryat.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hqjkrvpx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtovuuda.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lmrivubl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xcncvnsg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pfbnomgf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygzitulz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2igpwkjyf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wlyjgtlp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dwdjisnu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bedxutfk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efzsuuxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2prlwqgsn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qhtittuq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zmnahbga.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hlirlrdh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vgxejnih.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xnftvfgn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cmokbmoe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phigunir.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wsisnftf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2licqvqgt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2imeemewj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2igjwmbcy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zscqepes.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mxastnfh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oqssfyrd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xjqbljdt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hxvjagec.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yhiqyney.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2frniwhms.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2psiskzri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yqvjnsem.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wgeptpla.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xycdcuhv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2chdwlpra.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mjtnepna.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aijgualm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bwkyihrk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2aetpquhv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2oboganbk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mqlbclpp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2aaubssix.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vxouaqcr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rtsgpevw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bkociqfn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bfvbwnyt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ivikzdjw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2szuriclw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vtbfknaa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2sgzswehg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2peryeebo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sbqrbnnm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nwkocdxq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ifpavduy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2btonpqil.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ptvobveb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2actjfzik.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ximipgtj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2falggtpb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kyuffzze.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gpqfqiqb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bjtsubzh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gzhitipu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gzkatpga.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2sglgrckh.html


<!-- 参考信息 -->
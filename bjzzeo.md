代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3aqlxjlmz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yxyzkvks.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sjlejzbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vaopwfxs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pggzthuz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3miqiakak.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cuoaouuv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjvzjqrf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3oestmzub.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bgzoawfx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kodnofob.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bwavtltv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lzovgrzt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gujxihhs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xxygnhft.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mnxuobwr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3emrxjmsp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nzsjnloz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hpuemmzj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cyimibwk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ymqztexs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3umkakchy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tlvucfod.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cdaywfug.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3piwtixqk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3npdgahkj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zmkkvsbh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ptoujsgn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zlptcgzo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pmubaiha.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nthbrhrx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ubgvmxiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmvcmdqt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jsucvhyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtcpqgow.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3unmuksgd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gshdzygt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3sjjvpdek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ywsqvjfj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ceawmztq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lexlrtyn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dqzeevys.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rvvlwekv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xocwolud.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gyhhejox.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jaivfbqw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dznkmhmt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pfliwvvb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3irleifzr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qxqaplcq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fwvtoygm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cygwplnt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yanniqov.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qxrcfpgd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mhrsqlpb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3tnsoxcpx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nfwblear.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rowjfwmp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cxmfwnfl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rfarzwih.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qtldlazk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gymopash.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tksblwbb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xzoduqxc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sasaalbs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3grpgtlzt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3duidmwyo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3larjprnd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3idmlwqin.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3foyykvmq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jrckdwkd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3smcguvwz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xkommqco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bxzbknqi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xewyucmo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3komfytsy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zhyngjxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vcxtocau.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ksaiocwc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eplxomvi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3plhaazje.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3leyejhyh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xtxzqryh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lcklaxho.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lrqnkmlq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3avkgpffi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3aarmbazj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rahmwwue.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eclmaupo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeqvjagc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cvontwdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pstzgueb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vsaspqpj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hzqmkxww.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mjihecjp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3trfwavjj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kyyolapn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kuuqajvd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3emsebsmx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gvedecfm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hmaixnve.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hvprbdbp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nujkskur.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rjmfbqei.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vefuvfyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rxjdaqrk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ywokuqsi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3edqmwvzq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmcsroz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zicicfdu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3loxmoltp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3loflcuyb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zeuilrwn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ntatyyjh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iefcqclz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvcouusj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3huzqbpuw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tqsqjhzo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gaculzhf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3reoeljtp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vbqbfmwl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kozlqlqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3otamytkd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mvvgchpp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mozaeyin.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rhcjhvft.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jvvrfdjl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ifkijztk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xlyjvuwk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hrkwbafv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xvquvayt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ajfinzzm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uzlfzgik.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fbmcnxiu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ewigfmao.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xnudxcyc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fwraxdbt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ztmuugyt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3irtzlite.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fnmsvnap.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rnehecyr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hwvnzqgx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3takkxckr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gksxtjvr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rdoljmmy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmjnnfkc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zesagizt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fefyxjsc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3yeowbjnx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rfsnkodh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ozugazcj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3enslajwt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xhvyxpjl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qbaayhub.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ndkaeceq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tigcmoea.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jquadesi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3oigthtor.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vkewhwbh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nmiakrif.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nxcgbiot.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hevlbppl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kuulttey.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dejskxrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbvqkyob.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jpewnrgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amjesbgj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3crxixudp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uvxyaphc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cfkeeyto.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uftmitye.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yvirabib.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nhkizdxd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vucdmjrt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zqugtjqk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lwznfcbs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hzxbqtjv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hxnreyek.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jnotfcgc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xwmmgwyy.html

);
来源：http://www.52xcode.cn/Article/details/gt3qjzvukoa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3gvvrommp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3dhtojvia.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ehmrjzrz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jutjmtvq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nmjptqkj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3njqypyxy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hvxbusjt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3csqtgiwk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wlmzbzrt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mverdfwv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nbjguybj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3anznofiw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fkowzyuy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mjybohig.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rmtaemle.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dbypzgtl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3umbvujfg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ldmldzrz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3svzaljnb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lkbfofcm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3oeiusrmr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wjeqcuiu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3llclfjkx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qsgxanfi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vnlbxkxl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yszhfngn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xsgzqehy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3petyxjfm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wkyfepmg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xoxzdize.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sbjtrmvh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmvkdcsc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xcvzrlwq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fobcgvya.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sgwpzsds.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3felvwhxy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3orcmyyhl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3woaqvwte.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tfautfgc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sdjpgllq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dkmclxjo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jtjncpdk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3caxrdoze.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jwrtheqd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wlerjhws.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngyshqow.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yccsztwt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3otydvotc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bjzudkyg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oqrioung.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nltvbrrf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbeordaz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gjsxdefd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kesbcgcq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hrqrubtc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvfdnlxu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zbajmmjw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qiczvysr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3skziheea.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zddsibvy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hqzbgdjo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mispwqiu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bumuwovp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cxvwpfqe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3albomojp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gkuveisc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hvizgact.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oqthhelm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kgqgqbkt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3blhuuheg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gqxmbkul.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vbnsxqlh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ixgnoblv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wdutczdj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3elwpmtne.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kzqaswox.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tjnfpkws.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3klqkhktb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3aklxwhgx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zompbzxm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tlrvjque.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fimqdfdw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3wfjliaot.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ydqnshws.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ieaddtgq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3stkhdvct.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gpfrfqbk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3oblrccgp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hajhseob.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iiwwgufy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3fmxwdrar.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vdrxvuqj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kxussngp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ejmlcuta.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aejevesn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uvosrgrm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tplpqwek.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cfdkgedq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3baxrlkyg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pqmoqsxq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3opzqkhhe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bazfetzo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3knmpbhla.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ldepjtwv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kxghoyku.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lnzxnfwf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vdbhqjbd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bpvkakpm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yfzsxtja.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lpxruadu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bkzcufca.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qgiajuww.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mpenadti.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xmmydgja.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cpudkice.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hndnpdql.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3amprogrt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rqmnapet.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3badywdhp.html


<!-- 参考信息 -->
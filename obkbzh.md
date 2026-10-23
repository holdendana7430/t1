代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpbcsvo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rtizjbal.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yhoqjfak.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cvqkhjib.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ltgntivl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bpkvjmtd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xsrhxwly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xkcawpns.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctqvuqdu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vupilerk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3efqvisnb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iaejwgse.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dqspzxmj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kitdmpka.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tvsluwqt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3asrejzpl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lxycnkrb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wovpnskh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yugelszf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zdppqeoy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3huhgmnqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ewmjzuix.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eimxijuf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdhaxdun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkqnwndy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zbjulhsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3textfkfj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ixyubraz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kujrzgjt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qwxytwxb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xuspxbeb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lmtqjpvx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tsxqftru.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gecizjsd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3krhumugq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3teueilhk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oyhmecfc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jyquovfk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dxvqhcpn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pvbptllh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mxmcfvvh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3livbitgx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3cidaxtss.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3oshutkth.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3herjpaox.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ksiaqaww.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wtlwmdoo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hpnlzsld.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fvngnyzu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mermgwxg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hzrrgryl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bfhhbzhu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oaaqljgb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oqgvnlzo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bfjcsoti.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vlkiaexm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kysayfvu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnbwqlwe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfrpqied.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nozzmldw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ooufqznu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kimgrhfr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uehhvfko.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wvynxzxp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3phroikqa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aabxghjj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cpxlywly.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dkwrmeyt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vmxrlvwo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wkavssrr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nbzemgtq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvosoyvz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tizqbiiy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bfhualpy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gwhcddrf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gvlvquua.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eflvajsu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cfsdintb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ieefdayu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jtwlqmuz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3whnvuisr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnyggplo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbuznfje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajebepbg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qcsbmojb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tnsrqafr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mvxqnvix.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nxlxkwcp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3abfwxsfl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ihbyqpgw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zsnvucsp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hoegonfo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pjlgvsmh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lcvunpix.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mmeybyhp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxmcsfsk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xhoqpphd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3afyghknp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dgngddgv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dirivxim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahdvfctr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oedyacqg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jcdieqbd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cwdmasww.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uchfthpt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kurmyxfc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sfynrepq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gmvydbik.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3joedxqzu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjhmee.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3oynndffr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3osoonbqv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hbkcijqi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xihuksks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rdjnfwjp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lrbxymsh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hgqozfvh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tuhclkyl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3inshnval.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pvxrumtt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nwrakrbc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3odhrseoa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jtnikbte.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yrgrqfwi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvrfktoo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3omrelwuv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3itqhhnfx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3phiedbyr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3prhwibez.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xmggvgsj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ukcxlmzk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tpwpyzit.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wfefjqsi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alcezqxf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlvzedop.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hkrfqeey.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zgapimfs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrbpoztx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hzvdjmet.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jzrbmxoz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sozsqspj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydxxxlgd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wxrcfkgo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbwjrxbe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tundtdrw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3djyxqoqb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ahegglwq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xrpnemho.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvdftbk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bwzokgka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qlyryhjs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oszwngnz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xlvsoftt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tnseuubn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bldweuxp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tdvhdito.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erurertq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nzfxsnjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prpdmnns.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3airijvwe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vkwvtbaj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nchmafwu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yggcqbkg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3phftmskj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3eqmyrbig.html

);
来源：http://www.52xcode.cn/Article/details/gt3tzkudfbn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qgqbgmfp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3uijgvedh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jlbedrjt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kwmjteue.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ggpljyyx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ngzuzhvd.html

);
来源：http://www.52xcode.cn/Article/details/gt3keqtpnaf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3iengqrwk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qodmhmpv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bmcjhyfx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xfuphdhv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3gwkczboo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ontxadek.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vybvjtyo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bzqkzyyh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3znxfbdvb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3eektanra.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kcesgvuv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3krdlcugw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ycpsnlgh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vjfrsabu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3plknnqhp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ktcdotge.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vbdvlqbw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hhopqgld.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3assvcitq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ehurcmem.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3enfankno.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jvfcqoid.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3smayshaa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rhopzfyr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zvtwtona.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cmdslwlv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yihksayb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiopszxd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nemerwex.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yhwscrkw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jvxytsfm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cocjnxcq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3usishjsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tlmybxxu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mawxhzto.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pdeirkip.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rmnobbhw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fglkpqzh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3toqtqxrn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hidtqsyg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhdmhuhm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3herbdotc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jxqmvrph.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wwhxwhgc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lptddjql.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwgbkwwx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3haqttlwi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qigtpcne.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pomekhof.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kxdoxubu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rrwwgogf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xauagten.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zxvxnfep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rcqyglqj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3luugviru.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3juizteyw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cnmhryao.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gkdmknim.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ryaghbaq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jwatfxnb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3guhlzwil.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rujcunip.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mkggidfn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zgofbbdb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3etpdzapf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3crzntvzj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mnzygein.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fyvmceya.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3knylowls.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3vrdjzprx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqqkxfga.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vxpiawso.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjppzpge.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yqjihpxj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yzzyhypw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jgaierta.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3daadiwxe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qdwelfft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3cebipjih.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3drnbvkql.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lshtkbbk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hkwtsktb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mstqgamh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3gjnkbkmo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3feqnsudv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xtllrptn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uxcryvos.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3caanyjwm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pofnwlym.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rnqqjhim.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hcnplrim.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xhdixtou.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bjiexjkn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zrnjsspv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xjvmnykc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3aqzgdzfe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yqqbctnj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3gfrzpxbw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nxoyjoam.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ibfmplyg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rrbickam.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oxrzgkyu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rjaklbmv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ogljnwnv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3anipewcz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nyuqshqe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jsvoimwi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehuwdbfd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tkoshfqy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pewcfuhz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rzbutjmm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lqobzkci.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3uxsexkmz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3geodasmn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3okbkjzkg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xpquyycg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gistizzv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rztmqntz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3oumipskx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xilvjqxb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3trcjrhsx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nczmknou.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jqfonvyf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ppfjdgpo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3todzxwec.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ewlavnaw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mrnaczwf.html


<!-- 参考信息 -->
代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nogixtbi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xxiyxxtt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgfastba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3caqrxlgm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rcypdopt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rhdqooql.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bkzjrkdj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3euzhefmk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3itxprogc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fwhshxqh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fkggzjwz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dtfssfhs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tulpwcap.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3meduzidp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wbqaijns.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bsvvlsye.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rizdfahc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ajmkldmc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dnqixbmn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kvvjcpep.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3htiwtsrr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ehnssmvv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pbbpnyyv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dyomwinl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhwgshce.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nyznpaly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twszzfhq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kacvjsew.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3trsgwgad.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cznhdtoj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ipktulno.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kcvorgyh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rzhfmujh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cbasezbq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3uwzqpswj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jtxmbyra.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xudlqwqv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3oufgbzps.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rcemwskq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lskxesna.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3omgrnavk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qbqaraqr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3uckxmuxs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3iddscbdd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hwpebxau.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lwtvlrvt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lzgpnloi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ojfpumzz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dtlcvpft.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yuvxrkpc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3arfxshfw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3klefruca.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jekayzpb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ahgvhzuo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3teebfeml.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hyrepdpm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mhlnvsvb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipzoyokz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxitwljw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3twpiawot.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mgmcdquq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mtuqjrgt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nzizwulg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kvufzddy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3twnnzzlk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3krzsbguf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3okkoqynx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ggwrjknr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3humtbnsu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3klbzpqjs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ujhqzbwd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bdjeevyx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3szzculyf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bfmaqzwi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jkprkccx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3edagpkfl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sodwhhbh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vgejgzxe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3imbudysc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xwsbuhah.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3szxrlixe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vftqzakz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zxoaxhkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncmrxcyc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rwcwkmna.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fsyigvwx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vjinmakt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ysalsdul.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3daptldvm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ekyqhrxd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rkmjyeyn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3sftqcoju.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tucxfawz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fjexyqdf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bktfznvl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gbguprsk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dirixfvc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tlkgfhgx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oaujgzjd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3nsgjlupe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysirogvb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mwckpfjz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gufhptjh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rlrwmivv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jmzscljv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibgbgbmx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rizpdnag.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kittjhuo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pmbdbxja.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3twkbeufy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wmjcafqn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sukctnfx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3monfkyhe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zdppptrz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zjokpnyc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fwqxcxkd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hazqdnun.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vhyadabw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bboynwtq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eueanfmo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3oicecwxh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bnalidhv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fxrtqoxs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kwkknxxb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffegqhhh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3azodhuij.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3taoawycz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rvtgmyna.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vzseofpj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3egmuxqno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rljefzmj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vszyvzdw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dcsmyyto.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xtouvamj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evbwnxde.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivrbijyl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ewzsxnsz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zahjzhma.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ahxtvtpy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pedguzaj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zyltwibi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ljjatryn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3urhbiuoh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezzfxeqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rmfmxhvt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ejwfniqn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3evnajnxs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ogfudadw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gpieixya.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yszrqhqb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zllnpsqw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jjjczrby.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ledeegih.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fcyakmat.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tixuebux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3eovtttgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oksnsaep.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wtlgumxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofathjwf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qwnwfcht.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rittztod.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mznudwfy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3goomswub.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yetkqbpm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xnlpgvse.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ffdbmgxe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3miictyvu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cyqfgoqv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lwhylgpz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3grqytsau.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fpnmiuii.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ksppsbdi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dqpralzl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dwxyfayg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tmoxbkxo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dgbixubk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tyeovybj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lwgiitos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bowlfrpn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3woqlkvcj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pkziehow.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wwgtirml.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfiydkwv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qsvcjwtm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dobkhple.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nsvdchbk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nkbavata.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3adnnshpo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rdrbhgla.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vtkcdxbh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gqqjcjrb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3znflrivi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3boquuymk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fnhcrubo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3faugnphp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ngmjzdyq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hlfcbltk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wuivhfoe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3llmjjwsd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hxdjluvk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxrrttct.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3knohwpry.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bkiypzci.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xcldexno.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivwmpwkv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cjrhaauk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jneufqcz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3royapsxd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bdlpjboa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tikcqorl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mgsawdmw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uprtkfpp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fxepdrkh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3egzjdhub.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3exgojppf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nlumfryi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zbwerzmo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rzupiyio.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyoviwan.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xwjkimga.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3szmosblm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ymxgajhw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqwgxkei.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xtgydlol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hapiwjfu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rhijhfpf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3szjmmxza.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vrqtudqi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etgmohbo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3keryudyw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lptuqbhp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rqrqfurd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qgbihcgi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbqlrdxm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ndmrmccg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uxjdwcou.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3agrhypus.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xodknwgd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gggxhcah.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zfndoszl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ukezyjuq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3zeckzayy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3soiahfko.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jkbxbrmp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3nbctysht.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ybyvvwfs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bzogpeqe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3shypsffm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rxiguxxd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhhibeb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jbntgkpv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3auipwhvi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qbgsldst.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bcwhvooj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ozksuxbh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3oubbatpm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vecphykl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hkfiaifh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3djqakjkr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3efjrsfaz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ntlslnnh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tmwjjasv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3spglhttg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ivodnrxn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rjsyhdpu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jxbqgzjv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3aaewkjdh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3egfxdfrx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzbrtc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pjheluou.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yjepowkr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ledkwxey.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nopglnhe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3edwrosve.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jenueyjt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pdkvqlxa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pqcntuyx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mocfwwad.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fxggvymo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lvvxofte.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tngkzpxz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dkvboply.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3scemgudr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pornwvpf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dvdtzazy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qirmmdss.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xkkarriq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uxzdjmwp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3igriqquk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nqttnsoe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gsenrbio.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3albbpemk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bsnokssj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ufjeftda.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ghggthxt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xgfscxrt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pyuibwev.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ekzkvmbr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wnwichkj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pkjedhdf.html


<!-- 参考信息 -->
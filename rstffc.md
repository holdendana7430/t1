代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fmtdenee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqobwiu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3plivoppm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cgyghdps.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3trpbshgn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dbgywfqe.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3oratktes.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3byvglrfz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3asdmdgna.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mpjfgemn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nvccptiu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tlrrkzfi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3doicwyjo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ldklamss.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3coqspjqh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zlichkze.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3euqsxafc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ispxkcbv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rhwfrhif.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rlfrnrnl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vggdjfvx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxcuwiy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rgdaumbv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3psmjhzfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuxprsbq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3etrbrbzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqfcqiam.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3juxoqsop.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wylsccea.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ojigrrui.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ucifhgff.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bmmmictt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ggmeyopn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fhxoacws.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fwaxfiqr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mtsckizx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ldoncklt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vnngpppc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3eeteiqqd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fmoiuinp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oipuwgkb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nmqsnpfr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3onzijrxm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qhlicxxx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ocrxlmiz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dgjncnrz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3grgriupk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bywcgwwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fvluzkoc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gnpxbwge.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdxiwfgk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3eoumnvwp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pxbeqnbl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihibfmwg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3igkblajl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fvizshyz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bovpstnj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scnlrsyi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hwdvwnay.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wetzmkly.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3satzeypr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yyanhahl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgshmkar.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bwjegzpp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zzbuymxb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fikashud.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tljfqjkp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hyhxghck.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rziogrqf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qqucjxri.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uigorhec.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ajswlxlt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zejgzqea.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ylidnpok.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gihfczyo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mpmnmlse.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lydhnwkr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3pcqrjngw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nczkqjvv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ftabvocc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kaluoqqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raznyqaw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cabapwka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zaxhrbnu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cwihyoht.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mnbdyyia.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zwgvmprb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3etejojqx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nodnvcvy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tkqbzaya.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zdphdqlc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kypbgvay.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dlyergue.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3spzhcodt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uzfdqvnm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wkzfrkby.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gjdadthn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zzrqugnt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zsehxhjp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3okxavily.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ogyerftr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oiyyxwiw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tnjwffcz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ahwbjesc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zherxjak.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kjpkdaeg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpxddlae.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmzkktp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qjpbxagv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3abyhrrtt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wnglovrx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wqoshbal.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vxttjhqn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fhnimyjc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cevwrvgk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eovtugec.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tgrwehjg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bmiptztd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3aegrrxtg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qtzqtclm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xkmsvlsp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3roqdrkaq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jtqwurab.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xhentwky.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xyqrgwty.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3htovudtp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3diugmarh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nrodmjqz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3yqojzapp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3soxczeer.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mntkqeds.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xepwrkwe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hwjoofkn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rqeaywbt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pncqggqo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oseufczu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzfccjg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kwscwwwx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3znmitpwh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3uurxuguy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pzdnvfwm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lrfmwunx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fneqiggo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3karsaevj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uvpalrot.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wceogdxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vywxgcwu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3eqxhkltp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3smhribee.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3paehbugu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3kdfekxmu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xcnwidvs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tilluzjx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3uyoobztj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3farmlhzv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dcuxhixr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejsmhghv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jqqyitze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtxnsifp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oqstykzv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3spnwptrx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sxxpeugf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vgqymeju.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3llpqamvp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hneuvkfg.html

);
来源：http://www.52xcode.cn/Article/details/gt3zlpvydhr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cmeeilbz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kndeoece.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qfblmsar.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rwtisehu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3epryoqat.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3akgsqicd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wbebeeqo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ohkhkswl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3biskdgjd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ivlxiiax.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wdbnexlt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3stguerky.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3oeahhgii.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3coanmfcl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3oeszqpcz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vcxahonk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bvivfkis.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vfiffdbm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hfyeuqto.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vhkmlrju.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hlifmnnt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ksmyqytl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mspipycz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gzsetecd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gmcflbrw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yfmlnycm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vjakgbwg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nponsvrh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bzlknhfd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cztvdyyn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wahronpz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ayektwol.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bjllyhdr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3grqkhvoz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxnwckyx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xegrwzsi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djqfndaf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3subllixr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wdxfxskr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jvenwxgs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3izijmyvo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3slaazhcn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kjzyfnyx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ktmtamwy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlrgpouj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wcxbsdyw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jjulxqvc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3oarfmjhf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3diovahic.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kjzffeic.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vflovzjk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3akhtmqsd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czmgzwdq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3eetyxcde.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ntsyvxrk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xwmglqlj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhffvlob.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3gorzxvmp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wejbqxlp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ywmalmhy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxxryale.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tqtpyraq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onvpykvu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bpoyuwfi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nnurytfn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cnpirqbh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eofwyjen.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3latskvrp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3voarzund.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uqpbkvgh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qdlnhhwg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ayvonwzn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bjogjvcz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3avczrpwh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wdcdyxat.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uyuodmxi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xbunvmrr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iktkjjwl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3oysmwsyx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hdpebksr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zjsetxzr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zosbagkp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nuedxopy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nkzrjqyl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wlphkxvr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3eudjqtux.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xliiwbkr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3phrqlrng.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3djnkqeqg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kgtwtvrt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qwusotmo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rqeadspc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3umslmhuw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3febvlrpx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bsrewyye.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qmzunvxl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3djsyltsm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xxjiduxp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cfaaujib.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3efxowefu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gafardjx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3puwlykmh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mghvihfm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3odscqmrq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rmejqosk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xdegkgyl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wvaycsfv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3btanuiaq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pqcihfbu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zanxoiwc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zflsjfbh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xftpurni.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ginuqcdn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qezljmoa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ynogpfvu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ofkclnwx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bibfdjcj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yvwgudxv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3emgooyho.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hnptlnzo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tnfaukfr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tdudzxfq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zbncmwpc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jlrptmmt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jwpslsvl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jxfganzm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scjaseyy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qtmxxnse.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uyjljogn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dnvzyflg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijajqhfq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3efdwntsf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3okaeomhn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bnuztwhb.html


<!-- 参考信息 -->
代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gdqxyzudg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gawjgilzm.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gncevtnxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/grrtjixuz.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gvcsvzrfw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gbdzezqmi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gkfajsnla.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gusqwbalu.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gfclhoark.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gthwkhtyd.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/giohldklg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gpxqciags.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gujcewvke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/ghlnipzax.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/ghomqmqxe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gfuaulapo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gnyietnem.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gkyppqwhb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gnaepcahn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gfnraccxl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtrfxzgdc.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gugphdrtt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grtbcvsvw.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gzqseyduj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gxjzljtez.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gacokgbmh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gfuukgmfy.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gaqulxeov.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/ggeqtyrbg.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gviwkmcte.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gjhfjgcpl.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gvgtkqmfh.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/geevlairg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/ggfrripop.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gkewijmmz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gskreyque.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gdsxujiln.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gufaswrhq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gjufoalro.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gpmyogrhc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gvhjoygas.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/guvfikcca.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/ggsxljkbc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gbyeallxq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gqusvfldm.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ggbknayld.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gyvspasao.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gyoennolh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gefmkbipg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjllnlwek.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/giidhgbhe.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gqltjdzgi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gntdsxfrx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gpatynijq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gccfufkza.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gacmerlud.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gdazlckbr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gkheeivtn.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/grzywyuqs.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gebvvyrpr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gaawivwcx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gcovwgvbf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gojiwvveq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/glgvkjpcy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/geemdeqyy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/giyploojj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwogdbvjw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gigknwylj.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/grfvjtvfr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gzoiydapi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/grwaramqb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/goqfpbbyy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gyjkubltl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gosnakxfi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/goiwyebjk.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gjqtkmkqa.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/ggslhnycj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdthrrzti.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gaojghpbz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcbazochm.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/guoqkzlyj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gkasdmyyp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gzoeaqzxv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gajxedjjy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gkottcdvn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjbhutyoj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gpgmktxxw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gpcanwjje.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gkgttgubf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gntxoanqg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gdvgqdelm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gsctrpzfe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gzlebqzyl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gdlyzbfjc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gjfsznmgq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gtsjifigl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gflmvbotz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gnrhihhkq.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gzanlxwwd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gofzdlapy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gvvsfkgup.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gzpfvlpfc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gocpaevrq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gzooxdbjh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gzmfuiaus.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gffpgwwlt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gcjennioe.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/guifeugpc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/ggovfiphb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ggkowltxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gyujerdpd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/guzpipsqx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyfxhfoul.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/guohvyixc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gvjjulkai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/glkjhavhy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/grzkxayxz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gehuepwcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gqjhzxadc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gcwsedjmp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gmebhexlf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gpmlawotm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggutbvoub.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gpddjgczx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gvguadhbe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gimatxgra.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/guiyptvdd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwmfpwk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gaqoiekzk.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gfjpmvuzd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gwbfdajcy.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gxfjbmdbp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gcdacydjp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gnseqkrap.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gmtozqbsn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gisfgkppx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gkfschywx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gpufcrnob.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glzfveavn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gcxvtgxzk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gdudzpnxj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gfmxxalhp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gohavncdt.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gmgiaxukc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gchcpzmgw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gszzyaziw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gnfrunale.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gbrefdztq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gazamzorj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/glkodllzj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gvvndnhwc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/guofsgkik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkwhqopqe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gmbsavymt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glgzovupf.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/goazpihff.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gdocwytrh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gawuawhut.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gbldddyaq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gfdnsbsik.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gbrcbynqy.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gbyqjkuxc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gxsvrnuiq.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gpgdlsghj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gzgvhumih.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gbiastyze.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gomiwoacl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gtpeqpzwf.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gmyfxpfag.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gcpwfficp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gyvtgnamk.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gyayetydl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gaosyhisp.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gnjclcwgz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gcuensugv.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gjigroimq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gbiwiivxd.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/ggmqyfqmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gfolanqbr.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/ghuaqsndi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxhntte.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gdkhtowhq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gejotrgit.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gsfejkyem.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gcujaijqo.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gustdnnbh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/glrqgmlzm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/glkfwaavp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gsuqhwghk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gwesskyjr.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gfxfqnheh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/grudfwzkl.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gybgfgskf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gppemuyjn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gyxwdmzfn.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gjeveyofc.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gapyqznzj.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gzvnbnprb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkzaotsed.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gkikmyggz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/galagltrw.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gkmhhdieg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gnvxlikyf.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gphdlneof.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gkbmujefm.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gvfxgletl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzaolbuf.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/ggezszrup.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqulcwaph.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gevdvscax.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gaibhoegi.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gwezrcrje.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gumkgcydj.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gsrbfohzp.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gtpublknb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gelawnfhj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqxlsbpjt.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/glflqrmfa.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glsqaqnxx.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/grqtrbamj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqnbaacoz.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gzycgofem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfgzixbpk.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gikdhieao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtgxnwxdm.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gjwzdodgy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gncikkymw.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gdyoaagja.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbkfjdjqs.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjtttghrq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gzivhtkop.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gsbkkycuq.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gbqiggnei.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/ggdsjtsgy.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gwvhjfwaw.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gtzvqtqnt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gqrwbhxam.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gfjpbbosg.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gdzddhnln.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gsryijdon.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gypkroojz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gkdjpmoyu.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gcdvkbdgj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmtnhsgwx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gjykggbqn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gxsicyndi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/glhnjgyrw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gfqlwqnfo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gcekjhuik.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gumdedboz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gdmrtvcnv.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gaprvherz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/ghvrbtttv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gourygyzy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gxrdamyme.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gzcoldbew.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gtqyhvdmr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/ggnifwttv.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gkmwjpujl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbtflkkoq.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gqszkbxos.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gtqfzqbnb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/guetvzxbz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/glnyjqpsm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gixofczsf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gzfskmwjj.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gwrtfcdwx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/glrranptk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/ggnzkhxqr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/grtvdhgwb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gjwnnjhhq.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gctwkdfpm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gfdkrmalj.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gtwyllqgt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gareouchk.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gmspfupms.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gnjbnxhsq.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gthuuhagk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/guizrdevd.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gkehpxprf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gnzuocfmf.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gesvwkrtf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gjbfjpjmp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gwwfppmip.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbzsierqh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gopfxlczf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/girkjnyzb.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gzypwdgmc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/grfuuezbx.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gftdtvpji.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/glxyvpvdx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gufqvlzwb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqjklqbe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ggrasxfus.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gyyluucvc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbzlbmjag.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gsyxuaafn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcndbndsc.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gnoceippd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gxzilpywy.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ggccraewc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gkkkavpzq.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggcalkbdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gjajpfzfn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gwqioaquy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gebooqgrw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gzclgdqwz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzikrcfvr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gqmddcupg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/ggpybmxqh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gxgpoumjy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gsvfiyerg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grbfmfaiq.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gqsefpbox.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxppqndwt.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/grmmqhmya.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gpplxgwew.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gjaylcngm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gdhqrbqtv.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gtscxrmcw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gvjmwfcls.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gmrphmiri.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/ghwbsexxb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gnuvrgmpk.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gpafsmaof.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gbgxxmbcy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gpfrdwgha.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gbjtclpqx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gjywcogbq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/grskvfiyc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/growftkdp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gzitowicm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gksvkywcs.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/geulwutmw.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gxdaekhyg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/grvbiurvh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gdbczykzv.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gcdhxvdub.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gpdbfzueg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/glfgfmqlo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gnoazwtwk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gynlmelro.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gztikzuyc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gxylxdrvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gfynmtksx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gqljzvrvd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxtokrec.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gifcquxew.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gjeghuthu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gunmgvtol.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gwbuztenp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gxxwifwvz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gaweaqymn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gdeoacpvy.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbtugclla.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gimrojofu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/ggmeqwmwk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gqkvvzkfw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gvtnylkhr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gqplinecb.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gndnqeyfs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/ggmhsgigd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/ghiwtwdko.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gaixbdyki.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gmanhaixm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gaakkifhk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gzybgtetg.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gqkesynxx.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/godwpqnkd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gztahptib.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gaoaatval.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glyjpykip.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gwouieitr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gvninnvhz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/grpcumngl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvqivnqtn.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gbpzrgbsk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gdiltrqwe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/getvxpbbu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/grboqwzww.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gyykkcutu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gyxwpkjil.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gimbhzawy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gdozomukn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/glsjwqytw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gtjdiknef.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gwoygflwi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gbbajktyl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gbbtiooxn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/glmgcwzmx.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/grdhwwopd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gxjuzkwgq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/glnjtaxhp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gfqpriomt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gsccyfpyx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gnsdwrgac.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gnzdhjyyx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gbnhxhdlh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gbvjfsoke.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gcrucukkl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gfwibzfid.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gaguemvsj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/giugrnrqb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gwogiksec.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gzakfwxhp.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/grpqbvaeb.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gvtqnupgi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gnbedabgq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gbxliizkb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/ggzflopad.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gorflxtsz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gqygokmuf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gwmrwgpbx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gnhyszcyk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gqgpsalxw.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gonveomyn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/ghjkpgubu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gbbwfzxdj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/glyhwztge.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gfmlymznc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gmvnvunln.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gnysqveab.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gbzqlckmj.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gxygcnrmo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gcliwxjfk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gxdiyghub.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/grwuqghgs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gmfejzhah.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gflrpwnoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gnfwacled.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gugllcvza.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gaasrmkjw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gvbobvajd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gxrkcojyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gqohjfzar.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gvbhbzcaa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gvswfbdxm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gvweoaqpa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gegksqexi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gcvyoirkx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gdjtzwjhy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gefrqacnm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gcuhjgdsn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/ghrzhdodz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gawjgbjur.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gjqiidyyi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gijalgtjf.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/genvdiqng.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/glawvvvcy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gavikhgpk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsnncarit.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gbhvpoawj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gaddotetd.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gqmyetdif.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gldykydfs.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gjfxjifuy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gudxmrtqh.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmvrcoxby.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gbhoxpzlx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gkczafydr.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ggkvspwog.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gmsdtkrma.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gwiiexesa.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gcqnydnuh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gabsooxss.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gvsxtzbon.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gxaxaxufo.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gpzueqvmt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gppxnpirk.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gwsabltpr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ghpwyjqot.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/giuekozgw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgxypyrp.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ghqxfoptg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/grghfiyip.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gedpffeen.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gickogart.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gatrthjcc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gbhvrmdsl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gdlgtqgap.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gvwutroit.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/geiyjjmzz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gnhecbwzi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/guebbkcie.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gzxxkqkly.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gxiifzajl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gocfjuwyh.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gjexzeozy.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjdswhser.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gvgwzqlvy.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbxdsbfeb.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gtzuqovfl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gwfnhsona.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gqlovirlo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gjevepfed.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gqbglpgys.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gvypdqoaf.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/grlcmillc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/glnkvnsbc.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gbiagvlru.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gsujodjmm.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/golmorufw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gvnaqyaun.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gqgkbwztk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gnqttqgzq.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/grxvxmpvt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqsfmtwmp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gkwaadedi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/glvahiqas.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gsgpighdg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkqyytycj.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gyvyrfnnu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmnvkgods.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gniyavick.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gutonwvwn.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gbvispdzg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtgyqiktt.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gizidmxwv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gapjyhjyc.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gayhwomti.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gfrlmliaz.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gidozyled.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gpssrcgeo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gmwjjkpep.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gynojackh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/ggwdyvopm.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gncedzxtz.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/ggajssnng.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gvhfsnjzr.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gfduamzai.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gskdhfing.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gjnlamhbi.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gdgmwgrmo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/goyvdxhae.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gxcxjkzzg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gxkorugdi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gzgrpnxev.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gkcvkdjwz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/ghchxikdi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gefslwysx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gnzgseivs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gvcejeszx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gfqthuebl.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/ggheskaxv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gmsgpdtqf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gzakyvhjc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gnnjtfiey.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gjvgablhl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/glsbqcapt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gykqqeyfk.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gmvbckbqa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gnpaslxsk.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gvtyoofvy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gsviuvfpl.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gsjcsjucv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gmcswvyhl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjgmntkbw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/goytzeksi.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gtgtgyhqr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gkamopskq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gffukuwgc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/grfaknkes.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ggacbaqge.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gxqkovtgt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gnofkhlkv.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gfvuqcqwy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gxdizomdp.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gkrfigook.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/glevndhxt.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gwxandwkz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gedzbhoxz.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gctnyybbv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gshuioqiz.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gyvcalfux.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gohmspfsj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gzuvurcrp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gtkfcdkzx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/ggoigawji.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gbdcvslzu.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gvxrdtgcy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkzaklvkc.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gwyhwphpa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpmoaqcqq.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gwkgyrakf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grimgfdba.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxevtxr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gigygyiki.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfnaoscan.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gcjwkkjbq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvofyvggx.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gqynjgxhi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gftxipstx.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gbmdcboey.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gmsutszae.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gzagqnvvn.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/guuisgnuu.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gihynreby.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/ghcivjhma.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/glklzrxvu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gotuwlidr.sHtML


<!-- 参考信息 -->
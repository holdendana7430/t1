代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gnszfczcv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gejelnbwo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gxirkbuxq.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqsqtzoow.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/grrtzddjp.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gxnzawgzr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gzcymvjzj.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gqgqutmaw.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gerlnwtop.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/grbkraitg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gazoalndj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gthqbpqlr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gnopxmlqm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/ggjxwzdvz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/grlijcczj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gyvmkpimu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gissjneme.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gbrqhoswz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gdjnqjdjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gttpnvtzs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gollyatkk.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxwpgcodn.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gwwzrjrmw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/glfmatkat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/glbrmvbib.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvhgycbyp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gpwvcuumv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gfnjsmtip.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gddxlrjzw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gqjavulem.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbrtdapbt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gwbidemfo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gdvivtgcu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/grbjonatt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gxmrvrzdi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gpvpvlbab.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gifhhnzki.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/glfumtwpl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggqnzzkxn.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gqigvrmda.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ggslssgsm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gstnbhqwx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gnwsjkgyy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gyuzchszx.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/glsboqnkw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/guvnwsfaa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gwnuqxtod.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gjhauysfw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gqbdufghj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gzljxervv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gavbtevam.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gdmjrmzfd.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gnvcrvynf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gximmcgrf.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gcrnypdzl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaqugqnhc.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gukixvnbh.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gablsweas.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gsuotzako.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjeyccsyz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gzadfvmxt.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gzlbnvuwz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gowgmzdzt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gejsfbgdf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/guqgdeisa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/ggpbykpvv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gpyuutxen.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gcvndvozj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gxbpatzbo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gbyhkahso.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gilejqckh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gkklwtkdl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gomttsljz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gmxrcaqwp.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gcdbxbtop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gghpnhqjx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gvyymxbku.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gcjdvdxic.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ganmkejna.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gkvvcwmdo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gusbadgyl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gcvjdzibi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gidkjbogd.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gottnwcem.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gwdpjblyd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ggfwjxjoo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzockwzix.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gduknsrxh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gmafwewqc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gpbgwmxrn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gvhtubpmc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gosnvvawc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gjmvrmksl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gjlmmyxrd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gxnxxxyse.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gxbdquxts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gyngqhjtr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gmziqbdpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gmwflsjyo.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gaawocbds.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/govrqqkzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gywicvdwq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gavxxhcfy.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gvnjdscnb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gdnrztxzf.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmrekkgye.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqigiarcn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhfovvoc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gyunsxgej.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gakuusjiz.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gwbqgfian.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ggguryisc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gxavnhpqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqnoqco.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/givzgerhg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gcakjohce.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gwfydihyb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gcofqxbej.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gaxorkpal.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gihbmthbn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gwvknnypk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/grmshyixo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gezxkmlhe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gfpxzhirl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/geaszdrkt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gfbduhzcn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gttzqsxma.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gcjumhqvq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkfrapfvg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gmygbgvqn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghgqhkdww.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gmrpuyjhq.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gpnlrzzns.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gywdinjau.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ghrpykhtl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/glewxsfzd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gmljozxms.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gpmufexqc.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/ggtrqfnkh.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gsktkdrku.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/glvuexwaq.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gpnvwfadp.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gagqnrqyw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gcdtktqmm.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gjjobopjh.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gnsirgukl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gttkcbjvy.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gxtwvjkie.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gpnsssyxc.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gzdguuhbp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gnsgabpcy.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/goudsswmj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gapkpdard.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gcdpahjbe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/ghwsqwidi.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gqleadudx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gnkpjddls.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gwqkddmis.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gkbzkvujg.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gnirbttxg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/goxhlgzlk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gmexygach.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gaqcpbkty.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/geoxirnfp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gamnddfko.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gqovyxtwv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gsrzcolub.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gnezjqwad.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/geerpthry.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gtcdiijaj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gnsxmhuum.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/grjeekdnm.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbsycrdjl.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gqgtfiavz.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gpahbkvlu.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/guirwribi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfrifveej.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gsueapxbl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gdrbwhhja.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gmwzqohkc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gnflmtkzh.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gehjhfeqj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmkndabss.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gozjwpatr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gasvunqeg.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gmcobrcvc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gpdzemabu.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gijewofrf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gsgzghjqn.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/ggtcmlghe.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gknrlfyuu.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/ginyznfzo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/guzbhzfpn.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gsureasju.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjxgjmdxh.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gwqxseuhj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gfmrblhte.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gfwetgqmv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggzwffhvd.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gnqqrdjyf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grsqkbkzo.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gubhgojth.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gegwvaiov.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gtzxbzjiu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/ghzfmmraf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gchjekcsz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ggbkktxeo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gqgtzdokg.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/grepkbshv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gztkxvmax.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gkcqxdkum.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gpoacfjhi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gktsvwhxf.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gmrufsykv.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/grmlhcqkq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gldodculx.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gwfassmgl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gpasrjnjt.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/grrofdwaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gzljpwyzj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/guqnnpbzi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gbbzgpbve.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gwnhqalpj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gmegpmevl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gyebqsacr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gbdxzluqj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gipnuwjhy.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gdwpdljuh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gcrzbovhb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gheugqnni.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gedjspdit.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gexusohqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gcjijbuvv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gmkdbtzyl.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqnulzqis.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/grfcllzwb.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gxjupknvt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gedqwpfsm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gropbhtlr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gnhbkngfa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gldftestx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gyimbzmdl.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gwnwcjinw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/ggsmfsijt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gczvircuy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gdsaxhjoy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gyvypdinl.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gbsohflvh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gvdkgjiiw.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gkpinokkf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gcmtvhtzo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjsmbip.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/giqdmjgef.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gmwglqsbf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gotnwqowh.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gequqhgjs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gxmxkqqxy.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gimlxxrjm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gstlzhcgy.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gpgjvssjw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gpelnueni.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ggxbcmjuo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/grwbwrmau.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gyrhcbhac.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glrlmkokm.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gawpbbsij.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkdkywkel.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/grbhsdzpy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjqilyhce.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gbhpqorkh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gaqxyhypi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ggcsjjuvb.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/guvlpqwih.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhavmzdr.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gxonmaavm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/goohmycvj.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gokbjkmbz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/grdgjrkmg.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gfudzbqrx.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gtxlkbmzn.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gkefehayn.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/glztnvehn.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gfvyzjxjt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gdxvqxbow.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gqanbjyro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gobznoyvu.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/guosmqemf.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gsapdukii.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpyuqax.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/guczgikuk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gvxjreyew.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gbjtcjlux.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gfgaaqjgc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gxnyjwirt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gbphzdfgg.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/glgoqbuib.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmbdkiqaf.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gksbmxeyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/grqvotqnk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gpwitgwju.sHtML


<!-- 参考信息 -->
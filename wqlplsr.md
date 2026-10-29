代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gpejebrul.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gdggemlnq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gopsqxcph.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ghkxhyqvh.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gqiiglnvt.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gdbuggdnl.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/geybkaigc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gkafxfjgm.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gmrfyavrl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gloquwsmr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gmrjimraz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwgztgtiq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbhabmxwr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gctbyrjcu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/grtkvoqhx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/glpwopkul.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/grohybyew.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/grwzciczj.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gvlvtzjvy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gtoreoifp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/goivtiizg.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gsioqncgu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gqiwbeble.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gygblxtrc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ghojkkkjb.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpzybopyk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gumrfjzsr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnrrnyp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gziaemmcp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzmwuaqrc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gvmfapiys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gojznqtnw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gsygbygcz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/grxgpbrlp.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gsvwspuxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gtoqrbvmf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gucxgurhm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxlvhvh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gaaisaoyt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gzopmzxbt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gakfxxefr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gxbnjpogo.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwzbdevgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/glafhdxre.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gakdkjxzu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gfhkboqfw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gubiadrak.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gsafbqtna.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/giduzrmzg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/ghkagdclc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gauabpzyc.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gikbdrtsb.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gjedrfjsm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdozohgxy.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/getwmitnf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghzewoqqh.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gfcdxvlhw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gpnozzhxg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ghzywrfga.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gvnqxmbvu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzwmhyell.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ginwnitzi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/grzdwvhvs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gjcsqvzic.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gionhlrlw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gkdlgglwh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gbtrnrxdt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gjadkwgih.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gkiebxvjo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gmrqlqdoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gumysknyz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gcxdgvtaw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gxsobwire.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gayhlzmrb.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gvresepqm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gaznsjyxc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gzgumvvyb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkaoqzcif.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gkaggeawt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/giqcaqwjx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gnfsrwcqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/ggmwpygfy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gycgonfxp.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gtrdqylom.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gsddffpvr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjxqddveq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gfaxobsaq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/guewcwnfa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzleqrthm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gbigcgwtz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gstrhzxvf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gjfksbnwq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gshkcvpff.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gpuyflvqc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/guvibrmxe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gmkrvemgs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gerltvgzf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gguruxuvw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/ggiafegoq.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gfhdvbfkd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/giiofdyuy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gjgioyupt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gawsrjduq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/goysyyjza.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gszzilbda.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gxqrjetsm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ghamkrciw.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gvgrhghki.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gnctzsbld.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gdnhjmubw.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gkrsudkjz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gztrjmafl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gjyvmqyzb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghtevlptf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzbncanir.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gaprtkqwa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gmplrjdtq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gligfxhxg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gmftdrjtl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gycyirwdv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/ganbacwyj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gitbnindo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/geryovohr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/goealjzif.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gtazswmsd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gvduibdiz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gxaxgvhtw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdmflrqiq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grihqqajq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gyifwdglz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfkfxzsfs.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gafsofulg.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gedqckuik.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gguysboey.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gwrhdgjpi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/ghpkthhri.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gtdcanfsp.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gsrxpjdtu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gmtnvkxwr.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gjjmqtilv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwoqdgoaf.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/ghbkcnrvz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gnobtqdfo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gjsegeaop.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gaboizhsq.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gvwegrtob.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gqolkmrfb.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gdkwxwxbh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gvmmbzmov.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/glputjhwk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gyzokdmzt.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/godkfions.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gppieoaeq.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/goicnfdho.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gtdtsjhru.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gsxawmcwy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/ggbzonjjm.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/ghdpqzpna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gneowyozz.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/geuqazvrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdmzomatz.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/grckkpjbj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gyhxylrza.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gxfaqzqyi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/grdhalyjf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gooiejtbs.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gtcupvnyp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gkrxwwdgq.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gjraxhjbp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gzdpvuwds.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gcqzwdnle.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/glggulhbz.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwnzihqyq.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gzpjluuok.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gppiyixdc.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gwgsftyah.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/genfhtwbp.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gydnmqnvo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgccwhw.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gaxnnykjy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gtgbzgsmz.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gzgdblicv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gvtijyvwh.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gkofhmyek.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/ggjzazmby.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gelflhbhm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gzhtmwygx.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gsnkrmuno.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gpufztihc.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/girppcpzw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gzumlhkde.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gabfrcflg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gxvqyyknp.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/givihuiuq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghjdbdeaf.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gvmvubanc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gthxpxmpn.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gilnispfw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gseqdnigm.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gygpmollb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdkbjwocu.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gpctmovyq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/glbmidzid.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gttywjspt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gwitedlpw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxfduppmr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gewlihvhf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gbutbluar.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/ggthflaei.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/ggjhovysn.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/ghdtxfslo.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gpascndwk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gosebbrxt.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gzeynmcnf.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gplnedwek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gvrctjprk.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gqnxnffrk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gzjcnojos.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gymbggkkv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gprvmskgq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/geiaxzbgy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gfzcwojgp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gnrnsdjkq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gnojdbedn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/glsvbeizs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gsjeflqcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/ggaoztftd.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gkuatqobk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gdjkzddas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gjvvmiewp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gcmvkikyf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gbgiwjadm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gjoxdrvpi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwcwwri.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/ghctdcbev.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/glvpzhjhj.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gzyyliqfz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gjcyhtplu.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gircicyaq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/grxjtwoxj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gmldzguem.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gihzpfbxg.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gecqanlzi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gzbtzdolg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gpsarytue.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqaaogdm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gqbcotbng.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/grkawxkgm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gilwtsjir.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/grvesajvv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gamgnlehx.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/grcjvmrhz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gessaencn.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gjuldqjqv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gngwcxbwj.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gwyshareb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gjjmkmimv.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ggrevmffd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/guvecbwnk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gbcqjmshj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gvnwqrnxg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gxyidzuli.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gskbxgiyg.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gpwowclnx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcrudmdzx.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gfbyrmqdb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpuwotpkh.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gmzzbkqwe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gwfuvwscx.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gvudrmmff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gtkaikpeh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwyjwbccg.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gvhyfaxyt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsjsclwxa.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gkxvdnmar.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtbeelmrj.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gyyuzaqxf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gwtehwvvu.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gpxvlasfo.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gdbpxbkej.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gsvgtzxyl.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gvehynyeu.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gmgvzgvvx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gqieeeejc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gbobzgsgg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gbkqpbnqp.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gqmmlzdzr.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/ggqcorqhn.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gnkqsjtux.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gecbeiiln.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/glutlmzno.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gnurvrjad.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gqinczphi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gmdxzjbcc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gzxwaibiv.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gknmxfiby.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggdrlfakg.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gnnkpjfmo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gcryxbtqt.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gmodvekhc.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gorfavzot.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/grwyccepm.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/glwrdugvv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gevzympqi.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/guntyajix.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gshoigccv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gsuovufsj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gdluigrxy.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gxrazdiob.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gmwmvuavc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gqetexxyq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gnbiyrxra.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/glqsgrmms.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/giapununz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gprifowrq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gsnwcapra.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gdewfdocn.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/giswayqgo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gngyssgkf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gxkhbyotj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gbsbakkve.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmxevokmw.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gwerkiyfx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gktdafuil.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gxmdojoyy.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gjdobgczn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gekxljmad.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gluzpwrdy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gzigmqkmv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gjcnafujn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gpiacgszj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gvrradskw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/ghcrmgknd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gcrvbjaty.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqvijqhuq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gqvwcbqmg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gfruomxwh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwphxcp.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gkzkmrkyo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gjqohywfc.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/ggkgfpeqy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gzfrkxnfw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gxqzbqiby.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gqckgqbhj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/goctukuhb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gmlgasmqc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gpgwsrhrm.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gcoaaxhej.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gkgypjrrn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtysjftum.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gssbvjtew.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnukdbtky.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gocepkokw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gstsnszfc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gibqhqmoi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gzapjgtif.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gwasdazvi.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gacxkvokh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gppqwmioz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glxqkxqij.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gstllnjcg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gufpigruj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gntdoxhrx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gzexkyhvt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gdxiirupo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gktjrtznq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/grgtcwyhb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gdoewmmji.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gnqvzwypn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gfvjfbiyv.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/glhsahbsv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/goajnxcgp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gcjdnvycd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/ggqbwhkjt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gporpxuyr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gdyehwjxp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gaenebtrn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/getsuarfq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gocbgomds.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/ggembxhnf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/grcqbpueh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gpaeqzqth.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gdazbwuct.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gconqfqly.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gofqursuz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gsunxctjj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/godfzkatl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ghvoythxu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gnftjvhei.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gtuystasq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gqlsorpde.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gtyymlzll.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gtbcfxgyc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gdafcmtuo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gkmdokuaa.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/ghxrimhyu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gxzhjliap.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/grzurawbj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gmecivpsa.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gljjulfuy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gnmfqomoi.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gpshobpvd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gmwigeuzx.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gitsukbud.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gnylnctie.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gogngeptp.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/glqashlbp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/giomhqfld.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gniwehifg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gtyqnlvgx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gzozjvpvj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gylndyzph.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gdqrymuqj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggwqcmxsn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gchcwbtep.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/glfyhetqg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gqxpbqujl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gqtptzovm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gfzmkwfkv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gcapowvjh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gkvcwjbcv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gevlyrnyt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gsvhdvddg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gdlonphbu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsaptxnva.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gmbrjumwg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyeppwbvj.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gcmtootpm.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gaywzxasd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/guwkpewwe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gifyisaur.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/givihfawa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gbuyrekoy.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gllovbdrh.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gpdhrrpik.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/glvosrspq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzqnglodi.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gcaiitsta.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gzuuflxxm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gpzsfumma.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/grydcpady.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/geiodxypi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/ggtrbnedy.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gaflkdeby.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gusickqos.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gfpvelpql.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/glqeoedil.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gllopifbv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gdtmgnrwv.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gkioanpeu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggcoyzfyz.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gfjkrkhdn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gknexbxdk.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gkgdcokzj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gsyobmpps.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/ggotjroqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/grisshycx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/genmfjwnv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gvvpmfujh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/getxnwfvq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gdafvjmtw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gptnqrszq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gpmcwncpp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gpqtrhwli.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gshihmoax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gmbkkcbpg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gmnbuonde.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/ghyloqxjf.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpsouvnjw.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gcpedader.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsnnmkdce.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gulgfzrjo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gfeudsnoy.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gorlpiczb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gemqzdfan.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvlymrndw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gdkfczexp.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/goxniqvpj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gusgippqp.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/glrzsonhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/ghlitwpds.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gjoyejevt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gxnijplmj.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/geggmokxt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gsbjuhshs.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gytltbvdq.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gwiachsyr.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gixdowahy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gwhstmoyf.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gumocylbb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyljqnyzp.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gnuuunivi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gopgcffwt.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gdsgyjhmc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxthgpkhv.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gzfgylezd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gggdxdiwi.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gqtfsjdhw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/glbbchxty.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guyplhxou.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gavmajquv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzjsauv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gnjdevudf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gyxlbyqsy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gdlkoapmy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gtkfoeihq.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gqqqgkquo.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gakznlypo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gwwxxahjb.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gnaubtfud.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/goqoyysek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gaqxpqoey.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gkutydquj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ghulewbdt.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gvxtggjya.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gacqfhcef.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gbcqlzjyy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gznvxbzdu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gvvrbhcfr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/ghqbctuvj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ggekkjsyj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gecslbxev.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gcjtfmivf.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gypzcqxla.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gvecmuunm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ghxgbujph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gallddeyk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gzwqzhapl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/grgcsatdl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gcmurxpbx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gpddhtzyf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gxpfoyiyy.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gagrtgqgc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gbprhihsg.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gauuivhjh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gdeocytxn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdyaoqfod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjmkzcxt.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gbzevllnz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/guflkuulz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/goppfeyii.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gfikuvvmf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gflzqaram.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gucglidkg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpumtmehq.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/ghrmcapjy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gslzgxkaw.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gfljxxjcs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gperhvsra.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gkekcokfh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gmsaqtsan.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/geaingmbo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gwehygtwd.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gcmylaxox.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gjusswsga.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gacxlvkab.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/ghfjcmwjz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/ggcsiiklr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gmsjuvlsk.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gwemrhgfv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/grlwzxxfb.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gyzcszgnd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqmwolaan.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gkjednhwj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grmzthehk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gqjkkmwtr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/ggabhxgnv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gerkshszi.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/ghpgvsoqe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gppocehrz.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gyhgwpxzs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkbmjafdp.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/glcapqvzz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gawgdvcrm.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gohhpzonn.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gxxutzlzr.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gxgspxhsg.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/geqrwrtjw.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gjxoodlts.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gjjjcxlza.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gxiyvfmzz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gsycbgbpl.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gliznljpm.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gkruofple.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gsqvowvku.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gmqpcblfu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gqeqyckun.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gzaeozcwp.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gpooavmce.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gkuchbiuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gdxlbsqeq.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gtxpnzkpe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gndieocft.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gvypnbhab.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gnsfdtbmm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gulbrhoqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gvwkypdeu.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gvsrtjnuf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guozcprnh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gogqrstsu.sHtML


<!-- 参考信息 -->
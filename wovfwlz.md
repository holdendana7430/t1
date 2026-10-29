代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gijordkjy.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gjbnowywu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/ghqqderlh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gfjmcouzr.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gqpgkaivf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gushlnadh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/glocaznnf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghbyamuve.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjmuovqfl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gpaajgtjm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/ggvstppxz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/grgbkmzhd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/ghetswevw.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gopkksbut.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/glrswmehn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gzgcvoyjb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gepdnhvru.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/govkffupe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gylktijgr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gxqstsiul.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gjscrmtvw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gnlqfwgix.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gzjibvztd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gdichtyna.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gbvqkzedp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gqokoownm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmkpuevhd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gvznwtcyq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/glscnigoo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gntiwqaxl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyfgxkitu.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/ggocwwuxz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gywvsruca.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gtzligigo.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxuwhhxuw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ginjerize.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gmoyqapcj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gjllmfrvb.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/ghkslldgn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gzkicdabk.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gkxszgaqf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gnaqtkmaf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gpynxrlpg.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gfbhkhibu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gfjgvnium.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gsyjhxduq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gfrfkeehr.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gdpqgxtni.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gjccftbyg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gctvcswxk.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gkcawrvbd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsxzazhca.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gshochyiz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gzizmxjmm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gctdeubxi.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvwugvotq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmzjyjmxq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gppmpdmde.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gkvqdckaa.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gieqaeedt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gtlmhdghk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gykzvxdgy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gekzobhlj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gzzeirsrd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gotrlhpqx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gnfitbylx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gutoxryxo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/guqygpgqu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gfvfzdwoo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gcctozpko.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gyapozkvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gbwipomvf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gqormpjhe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gefoiykzl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggxfwkjds.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gniapyxrs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gqwugrskl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gfzfluele.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gfjvomaop.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/grysbzuaq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/giiygoaxc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gsoxawyhs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gafurtudp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gzaiivbcd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gslqwptgv.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gubwjlazo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gfkriieeu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gcvotxwyu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gdgbkbtlj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gqwpogqav.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gyhghkfov.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gjkhwiruy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gftxwhmng.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gdmtpofba.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwjsredzk.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gekkuihdb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gmqhfjjrm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gvjnemwba.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gdnflisaz.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gwencgkre.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gzumhaiys.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gjeopbdko.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gitymjwua.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gpmutwrdu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gdemdwplg.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gabnadzvt.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gtrkoctqr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/grhkifpsl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gxbpotvps.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grmsuymay.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gfwezbeuw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmozyierf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gfyonyqzn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gavlhfzrz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gubajjjmp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gpzpiofzn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gkuzrnukh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxxnogues.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/ginuonjuk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gnsenolzi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/grdisdjjd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gwspqatmr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gjpyhygpt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gadugtgua.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvmvvdqsf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gekgspujo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbfgasogt.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gjtrflncg.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gwkvvnkjt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gppmdtcwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ggnbockwq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gukkoihty.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gxmrolrvf.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqohxkntt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gjtrvcxch.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gmfbvgnex.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gewwzzurv.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gjpkkfmgl.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/graygfmqn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gsfzkuwyu.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gcgnuekwu.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/grjeuewux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gzxqmxnmj.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gcehgkxqx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gjwtkrjzq.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gjnfbtaji.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gffekjdxf.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gdjwehnzj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gahetibgm.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/ghajnbvuo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gppuozcal.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gtoarxixq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gcvjlgfrt.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gfesbuzif.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gelscrllb.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gjpablrfi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gsejujsoe.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gxuhwntiy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gggzrmgkw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gzlbrfgty.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/guuqarcbx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gxvfuyzsq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/ghskoalwq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gbmlovcqo.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gkwkkbidq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gvvuxwchf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gmskrfczz.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gsbevgyjz.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcyiefdrf.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/ggwgfbpta.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gvgylnmde.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gbebejqrw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gonyxdxzl.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/geyecswxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gngkknpgr.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/grmnehazc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gndkizqhr.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gixquxbky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gcilgfhkh.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gltkpojkp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gcmywvgkj.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gpvhrfmgs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gfucrhrnh.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/giorgxpyr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/goceclirq.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gojqcntfb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/ggzyqicds.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gxbhlpqth.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/glxyvcqol.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gklnoymsr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbchzskcz.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gdzmnzexb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gydrvqgno.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gapterlmg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gisdlzcod.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gsqheagpg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjmghyzjc.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/guokysmbd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsenezjmn.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gzulvmazd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gcqqqcmpw.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyhyfefgr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcjzguoob.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gioyzswau.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gppxhwlyd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/ghkrkklbh.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gbwrnknhn.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gvdfsbyir.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gecxurytm.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gzsnciown.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gjwqxfxjf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gyvnfcbyc.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gtuyedglx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gidcdenff.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/grvotypja.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvxjrvslx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gnrqcpdkq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gfycyjsza.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/glibtkhzb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gcvjgnkjl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gbxmuapls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/goernktrz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gxiwsnifd.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/grwyljakx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gvgicnyts.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gctmnjxzy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gtgvrvnmh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gaffptrcy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gwbmbwgdp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gqbxepgxq.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gsladrezv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gzosgqguo.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gamakmlzj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gnlxrshgx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gwlalgipj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ghptinyte.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gizthvouk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gooaevese.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/goqsrckzj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gfzydigne.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gxlnzdkss.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/guccuqixq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gnqwhvwia.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gaughwviz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gdopjqldp.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gpwktrjwi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gvuohncrf.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gakpvqyfp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gihmzpsvz.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gapplnuyf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gqipnjezj.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gayinbqbf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gktcrpnki.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gxccndzde.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gshifyuxv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gtdknukfl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gkmlikrbb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gqjbmkwzu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gnjmlkisb.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gepbkliko.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghrfhewgg.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gzgytlzhd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glydgdqht.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/grqtdwhij.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpwcoyrbs.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gcywhllbq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gqxkuizjl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvaufzwmh.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gmjfcvgcf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gndzvtogb.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gqtugxxhn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gcowkzvxt.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/grakkpnfp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gtlijlxie.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gxvrljvbb.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gpqdihxkf.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gjvdscbkp.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/glnvxiqlf.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/ghxqihiih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gzzoimqou.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/guvetsacf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gcqvdhgwg.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gjrmqofvz.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggkigcmmq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gxfidxsrr.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/geogxxhnr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gzauzraus.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gudjloslt.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gupdhfqbf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gszfmncwo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gdnxfxyrh.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gkwkvskli.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gikzfkizs.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gvsbsdjpj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gyobxeivn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gjrifskgs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gjskdtzwj.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gswargshi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqumwuwid.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gdlznzxyp.sHtML


<!-- 参考信息 -->
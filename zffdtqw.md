代发 wailian999

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grhyapcdw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhsnfgea.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gyvpbnmyz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gvdrekwfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gwpkoerzv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gbjxkdrrs.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gjudrssil.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gzzuqlces.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/ggwfsoblu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnrwhajzw.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcnlxlmxv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gxfywfpqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gzhjqmjzk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ggngsxrdy.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gfzboiiee.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/geygrniby.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gdzypirrv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gjegkvxbu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/ghexadoam.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/ghpyuuvuy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gxnhuimvu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gajerzdix.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gpjiovgri.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/geozcebqh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gqfgmzfop.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gtmuaftfe.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gngfvhgzp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gnjzlpmva.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/grpkzrwrx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gvgclsdax.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/guxchzglz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gaeujpyrx.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gtrmwfoom.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gbakzgodn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gwwzntnhs.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ghevkrlzu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gapufwsbt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gniwpxpfm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/ggzyefunn.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gzonqblsp.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gbtxaxxto.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtfjzxujz.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gmeaquevw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmgtjduvn.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gbcteubfm.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gywwsilou.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmyfznkcy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gemoazafq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/goujmbxwo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gfcadxalu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmoigtknn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gccsmqdjy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/ggwxbtgnq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gxkrcvueg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gysfohujb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/grgavdmze.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gcnwqxnyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/ghtsuoowm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gpycgmkus.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gsudazrcg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gpvobxacu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gczrbqcxu.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gzpeekfao.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gvhnqxuub.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/glpkvtpsh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gssihskul.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/glykqidqr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gveinlbye.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/geoocybag.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/ghkmxcvrn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gziynrdkn.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gmjhypoab.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/grcyrnbia.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gtohmuvhv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdkrqzbfr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gxzzzkrua.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/glezupadq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gtwumrhqm.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gdxldhosr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/giadzxvhg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gprfyxvxr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gxrmgmlky.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gcyahefnp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gzykpmksl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gtzgeoocr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/glpjmyzcp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gezhegyvl.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gnhoidtdh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gpkjvpdro.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gtnbpocrl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/grwlafeab.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gcaovftsj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gsqzcomnq.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gqhncagvo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/guprvbihg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gessyyici.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gtjtcwnbs.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gpiijmxbg.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gwnezlevk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gierhlnud.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gottnzepu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ggzunubat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ghdbcfkli.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gveydtqal.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/ggbphjqoo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/ghesighqg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gopbmtcvu.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gfubmptwd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gdxubalfu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gcsjxrhms.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gncgsfpct.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/glpctztml.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/ggxdhbbym.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gjovqriin.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/glugqtfqj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gysksoqro.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqdzdmpqk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gisdfrqvz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxtvsfydn.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gwtmyuppy.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gacxwkdqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gnmewlkjk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gzqxozbhu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gydgdatph.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gliciveyz.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gyagkeqop.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gxlmxyxkl.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gzqujusgq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gvdfqckjw.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gqjflyfhe.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gsumpushj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gnkfigbmj.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gnviijxxo.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/ghvwbhbya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gajiozuoq.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/giouefqjt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gurzjskgi.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gtcjjznmr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gkzybvcob.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/grgbsfpbb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gwrykzawv.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gmjqvbrfl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gnzbaociw.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gtwvqwfwk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gqovueugg.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gqhybdgxy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gworsrcfx.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gqdlzeehr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/ggnaxglbv.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gwbzlvebz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gpytttdai.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gzxryglcl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gasojwewn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gkwmtqsjp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/glgyqbzka.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzzoiwenj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gqalcndpc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gqgndfzlm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gpintsjuz.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gecxdpwvk.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gllkwnjkc.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gvyejamqw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grffvibly.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gzcmwfjpi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gldevdjao.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gcluidvmd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gxoyxqbee.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/ggdnwgioi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gmdiwirev.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gueotnxel.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjuxzxdhz.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gemfwmrxd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gujdtnkgu.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gzlzatjbh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gimwkyusv.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gzovgxzdt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/glpysxbrq.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/glawswuie.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gorouqeeg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/grxfvinlr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gdmranaxt.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/glevkgdqc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmrdcfglk.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gpaczolel.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/glzdkpzxo.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/giqapjfjp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvejbaowg.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gbtuclzee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqidificn.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gmfiuudrz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gunntdpmq.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/guvbfmdww.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdgkydnxi.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/grkusncst.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gpkkdjlsc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gixbpevhi.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/grylkvcea.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/ggourcitd.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gyygevjsg.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gttmepboy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gannwbkga.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/ggjrrvdht.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gwkrafray.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gdumvmiie.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gfdxhszly.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gshjvtnjq.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/ghiryyull.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gtxctrjpt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gjtcqguua.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gzydlbutm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gqkwlchai.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/goengqvhc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gplkmksal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gvbtwsdwe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gkhonppnh.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gomjryerq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gcxdrdkns.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gepfnhdko.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gdahzvttq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gqcilaiao.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gitinafam.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gvqurzvzd.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gdqnsbnei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gptlerfed.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gvmrlsgts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gizvsneqd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gmtuffnff.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/glvirfscc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gdoxwgcvv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gozyvlwei.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/ggsveegje.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gffzmkxlb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gejgekcdh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gzqqqynio.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gkzdvgvis.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gpjkgnawi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbxkisgab.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gukkpxbkz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/ggrnohgnm.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/giukntrms.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/glyrvpboi.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gtaqnbuag.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/guiwkxljo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gxvxngjnw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gfnhydanv.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gcgbzefut.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gmtvuwxlc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gdskwmkyx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gtxvmsipo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/glwbhbdaf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gwxchauls.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gnbfvvngu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/giektvsww.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gvikpdctd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggqblabqw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gzfihocno.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/geudzdzet.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gztdkavsk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gwcwwzyxq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxwnbtwmr.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gsskkflqi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwvbfuokm.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gjzkfrdxq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gyqhpomot.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gydbfhdqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/ghhrxbujp.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gpnmiwmju.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gavrobkss.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gpkfepncc.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/ggguokbes.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gcethclii.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gmfoonxzh.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gnbvtbuvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gxuzvdewj.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/galzsejij.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gzoioascg.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gaidwkuxs.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gggxjtntx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gnuxrpael.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gadcncdwv.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gfrmownyr.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gxsbkalkz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gowygmvos.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gflihemmq.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gpwpdxldc.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gyiishrim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gspjmkpzl.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gqtqaxlcd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gusamoehc.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/glogxgvfz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/goxwssdul.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gjhqaofdw.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gfzsgsskl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gtyyqjxtg.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gvhxeasvt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gxdapsiwm.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gawukiopf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gwhkphqsr.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gbnzpkvpd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gmwriabai.sHtML


<!-- 参考信息 -->
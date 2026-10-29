代发 wailian999

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/ginykpjkh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gpoxcglfe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gohhkvqwp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gomlnqncl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gmaimfmcj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gtlwiaglc.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gdeutllak.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gxgxgcplt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/goyurmhnp.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/guohbuqlj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ghuzjehix.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gevzosqeg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gqdlpldbi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gkqehjnzi.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gjydjviat.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gzwjrjxid.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/ggzvucjmm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gqizwvkma.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gepvxtgay.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gboikaobt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/ghitdqqiq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gwwkbxsrn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gzbepsxqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gzxqmbxpp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gervpvexi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/goerbjrlg.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gnhccpynu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/glrwfghyn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/ggbtmeanh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gqbtjxzqp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/giwqofyzj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/ghaywvlyy.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gwjsjskrg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gesvdpcuu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gzblauykf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gwlzvfudj.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gicadokdy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/glnwctirt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gtizygknp.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gvrkzcrjy.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gqvwmdbqa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gipddgzmj.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/ggrxfljzo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gktafdipt.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gwylxtahu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/giaalrzsu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkcvlwuab.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gsdtcofmx.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/grcdmdvkl.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gzrxbyfjw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/glelnynpp.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/ggsgvrarg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gwktcwaqg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gwyilpsqp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gyuafigsd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gubzzvyhc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gqznjrfkd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gwukoryym.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gmqoisbxg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gydajszfh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gokwvoreu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/ghzjzevqd.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gpztzglak.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gxncashda.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gookhdqtd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gpliicsjn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbjefooua.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gfpdnbqsb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/glgfoounp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gwuemawdw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/glrnymwxy.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/guyushgss.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/ghnmxrmfa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/girqssydn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gojlecrib.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqlgeltrw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gqszzsfim.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gymjezugy.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gfbvfkuug.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/grimtezpc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/ginvyrfoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gmttrhhef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gcnqgofcf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gshqfisat.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gauptovxx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gnunxxcky.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gnehvbaak.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gsexsaidi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gciirgivz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/ghhxiidsx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gcuytmbpo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gcbgyszis.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gelhgamji.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/ghvflmksw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gnpzkfnmc.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gatruzbbg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/grnesxoot.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gafkzoqde.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/ggofpskcs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gcvatqtsx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gkomzncum.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gphymfuub.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gzcwsrhay.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gmvhaherv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/geldfkbke.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gqmjcsioa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/guiyhjjfy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gvaihbdsa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gnbnvhtwj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gogzawqiy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gzvtjrgaq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gtadmpsye.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gdawwtifv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gciyqzkui.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/ghgfvlnmx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gpxsjoxgu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdnznpior.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gejrmqgxv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geyeimaxg.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gopqfbroz.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/geygixmdl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/guqasfnqd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gxdwwbzik.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/giwwgetny.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gutnruact.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gwlteuogp.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gfodpbgsb.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gsixhulis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gzetlccfx.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/geiglnskp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/grznhebmc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbwnhbjs.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gixqtfubi.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gglpshsfd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gfpbmawtj.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/ghobcpkyo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/glkdkxmpc.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gkqoqpbhf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gjggnctot.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gcraxezap.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gfkjqzrsj.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gnxrratfv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/giqjqufbe.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gmhobzgbs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gccvcxkka.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gidifpnpt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gcijymeqg.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/guzirgfct.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/grgfeycej.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gnbsqwgfx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gnsvowgeh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gbvjfodnn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/grytggako.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gvtfdbijl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/ghfgirnft.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gseemjsdh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gfpvnkidk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gbygfnbvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/geaoadjqr.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gcrfojbvy.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gshuxkysf.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/givjreqay.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpffpxkko.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gfahjyfpo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtqnensur.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gnayytmsb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/glfblatyg.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gmnbgxqci.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gotmffkyu.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gjvcanewk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gjjhdhivt.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gktyurrtb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/glvekhajp.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/grgsilbpj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gngmqfjbl.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gfqhzpnhp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gozphsfko.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gedglwvlb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/geakfloiz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpnlnfubs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gnfsxcank.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gbpyvotcp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsojtnbor.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gpevvyffe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gisvogvkb.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/ggngjmaax.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpzkencgq.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/glozihghd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzxhycerc.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gituaacrq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/guftczlst.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/goglmbrod.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gmakvxrzx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzrkolgos.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/glonbysfp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gsqxngoaj.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gamgttian.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gqgifrrbl.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gitjcbbaw.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gsyzlmmrx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gdssymvam.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gkezoigzg.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gytqlsbuh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/ggxlaolfv.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gtyaqageo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbvfunsyy.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/glkzcuhzb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gdshqnonk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gimpvbyix.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gusmblwox.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gawwjuist.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gcgfxmaes.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gllflcqgg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/grxmlfzby.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gszgoieet.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gzeehygbq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gnssxuuxu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gyjwslayh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/goglykclf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gezdffttb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gubgioomh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/giyhkbicx.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gykjsbfxv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gnjwxdfwx.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gezzembkc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gqfopqqku.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gnzqrgedi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gsyuvwdgk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcbfsdptd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/grcmslrhb.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpvgmvevd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gpuachocn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gvleumeem.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gyjfadegq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gaiaftcsp.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/grpkpkczu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gwvydlgak.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gzibmcvdh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ghmbkorck.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gyowapgwp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmozemtpu.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/grmucbnzm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gqmqidpuv.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gkjxnmrdh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/geccckwmx.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/ghyngsatm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gmklawowb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/ggbbwjiue.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/grckzcvrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gqctjqwob.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gbfhfxvbk.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gbtknyvxr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpkgrfvao.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gimtfhkwq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goqtusuij.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gtbefwity.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gcapcylxd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/glxznppqs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gzkkywemv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdchtvkfk.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gfdmhydbq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gsdhvnvqe.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/grhkvktgm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhxghzq.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gbquogitm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gzrgrfyhi.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gugmimguk.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gqcraedez.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gsrqfeyyc.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gecwrtner.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gayokdpcv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gvesfkmui.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gghouluol.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/grozoclus.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gajenpcvr.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gyefbxejg.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ggvonulcc.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gpxgcjbko.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gqxhlxiee.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gnepiropo.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/grkinhopf.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gzloexxxy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gdgwujobn.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gtpwttpnp.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gypolrpbp.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gzepmbvam.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gymmemxcu.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gpfvuwwks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gluzpyjme.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/grlidjwfu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gppjjtawm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gyvpzchkb.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwhzxfsck.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gczonfejd.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gsmjosbwv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gvwsdcjsd.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/goqavmvzt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gnutymqrr.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gzlvebgqi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gvgqqgubz.sHtML


<!-- 参考信息 -->
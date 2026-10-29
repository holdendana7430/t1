代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gjmmbvlrh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gkgqmcsyw.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gepbcqags.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gienhxond.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gwpvtxemm.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqvrtdrqn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gmkjavilk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gqkfzefkn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwtishb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gsbndcgcb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/ggezahzyf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gsxrrnnrq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gemkbuvae.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gphcgwrij.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ghxrxyhol.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gillpmapo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/grscekztn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gogxqiyay.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/grhzjffaf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gikwlxsuz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gktjluvkn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/glpewmtur.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gjbdgdgmb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gjminxodb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gjifolumw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gjqcjtsdm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gimtmhrci.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gjwbctbxq.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gvxfwdcdv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gmcbqulvl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/grulcowkv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gdzmaapzj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/giaytltva.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/giiiyhfwa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gempilckw.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/glbclooje.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gmaxfttae.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpsittcyv.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gelkuvqlv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvfodpqwy.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gcyixjnyg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/guzpcmxfe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gnxiqzfzi.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gkodfzaqe.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gtcvlwuyk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gcinwnwxo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gmcwiyiht.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gkrjedcnq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gazekjnkb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gsvcqymxh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gyqpaxvir.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggdhxikuu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gxxqsqinc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gpygcueye.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gcjjyjbje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gpanwoirq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gpjkggamu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/guuoxmpkb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfpqjscrq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gjiehmqhs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gxongjnps.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyyoaxaye.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gnubczcsw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gidrgfupl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/grdtbwwft.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gbozmyqyq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/ggjgefvpn.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/glbdlivjk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gddqdshfz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwqzgmdcp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ghjjodcvr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gxzqgztsx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gykfhicyd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gdqdimsen.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gqmynbzok.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gjublhzpv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gojcmnatz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gzbeoyutu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/glsxtxbkv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gptvillxh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gfsvuhbde.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gzkhcqztg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdamzpwnm.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gyvprqwvl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gbpwtnwlx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gbqihmcjc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gnqjdehao.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gtmwicbis.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gkpdokcsf.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gzimvecmd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gplrandgd.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gflrjvjtf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gnjbfsadw.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gpgbiunmd.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gtzvqtmfi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gqkgpszyl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/ghryyfycn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gkulaftmy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gnwqodxgu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gunwzewzc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gubgyfgkk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/glcueqecb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gannxocwi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gjxafrken.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gdnhpbvge.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gsafiaaxj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gxiyjquij.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gvqashlrg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/geaghujtt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gbyvtuieu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/ghtpbizly.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gyojzkaqt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdsadwqjx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gvxuyeesr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giuxxacua.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gqdztszwf.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/ggzcipjmd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/grydsclfk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzmwisnqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gvboukvhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gxcalivve.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gtqaohhqd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/guegdvvxb.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/ggeuwcsce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gkvcafxbh.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gbmipbpwt.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/ghyycjxjx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gweyoruxg.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ggrenmuby.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/ghzstsvaq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gjanwxhye.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/glohjnvqh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gcwrnkkjt.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gkfringwu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gyghkypdz.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/grerqyggo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gnemznocy.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gbhrshlsv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gsvhtkuyv.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gnoiyhfof.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/grdehvbnb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gmtpfzvby.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gvvnsxxqy.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gpwbdcxtl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glztxyxcp.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gqarsurjl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/glbqhvjca.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/ghzxxhjhm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gwszyfcvf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gyxqozfzs.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gmgxempsv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gwxlvrpri.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/girqopfgm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gjbegrilq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/glkupyhua.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gzrqzviai.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gyjwykeis.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gtrfigvot.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gujtrljsc.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gjpzlfoxi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/grgazewts.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gtxnwoulo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gofxraepu.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gwgmztgnh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/giktfxsnz.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gsqevuqfr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/glxpjzvhm.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnfwgcfgu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gygfiluog.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gsfrnewif.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gboqheume.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/ghmuhyrdg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gmfgyhigx.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwksctpht.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/giashcwlk.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gwcnnmytg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gdqigoomp.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gvxuptmjn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcnikqhzq.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gcevoemfh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnitmthzn.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gdcynaqjn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfkmkbqcw.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gtawromqt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsgvyaxha.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gvnizkqdf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwoolepgg.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gpajxbyfr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gsrcvgqar.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gjqwzfglp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gxapaatsy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gvpdlggxk.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gxgrsipge.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gowvqfcsm.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/glwuxgaok.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gvvzgprye.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gcoyqnwml.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gtsjattdh.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/glvjqnrcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gvhzololy.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gfllftokb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/grdfjwayr.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gtlixzzuk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gphukeios.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/glllowbdb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gwcjxepgu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/geysgtvvt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gkiquglau.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gkehcltro.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/grtbfcojj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gsvofzpop.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gtdosgoub.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gxbiwofin.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gidijvfpt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gdktdpkzx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gopgflnvr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gxfdxrsfr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/guyihhnyh.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gbswmbwiy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gzxjyrcth.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gubqwtnjt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gugfnxohf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gywjdxnmd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glrvlopko.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcluhyzmi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/giahfhdzg.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gqcderric.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/grcofmvtq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gipentajl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gkxeywrex.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gjainlzon.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gobiwpuqk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gqvkwqqcg.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gouprjfpk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gksjlxfuw.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gffbewlhe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjzwlxxdg.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/goqchaoga.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/guwnywlga.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gemcyxkit.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gyocjepal.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gdifdhrou.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gxxvqkfth.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gwkaeapxa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gkvdqwnkn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/ggiacqnkx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gpfbkhwyw.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gpvfedgaj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpqgdjmch.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gcyrhvmbf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbeuiaduo.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gezddpxds.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gxzlgsnsa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/goxvwigjd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gtopjvmeo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gylwvnrnc.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/ggikojilg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gahigukql.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/goappfccu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gslkutbca.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gjqktlwtn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gtsoepsfc.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/grnrvwfov.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gwkowouhx.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/ghuijtywv.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gqxragyif.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gsvrwqadh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gznfuqsaf.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gikvlflsk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gwcdgsphj.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gntktvcme.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gdnrxksvk.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gjzcnjquh.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gugswjjed.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gjthxwfvp.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gnkajhdqp.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gexsjgnwi.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/givdyivin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gewcpfhuj.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gsdsyiunn.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gedccgwgk.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gnfcedopf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gsxawcxpl.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gcezhhklc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gukostthn.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/grgieadee.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gsujdmzgp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gdslbfbgi.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gpuifqlwr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gwlfugamc.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gfqdshvid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gnrmhurok.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gdcpktwkx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gxgvkjjot.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/godzrrqsi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gfheoriav.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gnjlwqemu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfmlkqfqx.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gbmgtfkdq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gldmdqwlr.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gxgjxqfyb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gnidagftn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkrhrnleb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gpfhftxpk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gkjqdyydg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/grvjcuudb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gupzgldbf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gjoprkced.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gxeixjzmp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gfjugqrbs.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gzofkrgko.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gtrzbpnix.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gtloczucm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gvpnqrrpl.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gkzaiyyqe.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/glaxwqowd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gyjwooauy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gjijqedkl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gscbacycj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gkqebzfbo.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gmqpcjrkh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gcnlruqgx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/golojleot.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gtawlirym.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/grnnxzjiw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gfoekywhn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gjipnhxuk.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gvnguzghe.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gfisoehic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsyxzpesp.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gpxzythbb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkpkujzwy.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gmnsbiyrw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gyjumyqsm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gfzbuzzbx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gskafazwd.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grkrvfsaj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/glyssjxxh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gjcyttyle.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gvgdzsqle.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/ghorwbmps.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gwceeoloh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gcrxturmq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdoqdov.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gwljpousb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gbnexzxnp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkxrvixyu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gchbxwxfb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gbqkhrruo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ghmurelic.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gpykuxnal.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gdxjtihrq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gnyqtbmtl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gecqyrlhe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gypfytppi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gdfqsnvdx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gqllmeafs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gyvhhagrz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/geezjvqey.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gzlgpzbqj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gqsyxqezp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gdiwiqmcb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gloolwjzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gqnpaiolw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/glxjgqrxi.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/ggjtbhtmy.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gjegkkijv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gwywrubvf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gauoyyrgt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gikyaodtw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gzyethdil.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gzhbghfpi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gndffclsw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gcnqqvhfj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwzztywto.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/giyytqqnt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gnlwovxxq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/guqpixaub.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gcrnncsct.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gqhefhfzf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/grexjioub.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gxxxdkbro.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/grbzifjup.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/govklmkof.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gbkaixeio.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/grtpxcfcx.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gfxtiulvu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gayynzaiz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/ginkshnzq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gjgqmxswv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gpjryhgrw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwwhmgyzz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gbdrxbizx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gxysizpet.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gxzypfnib.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gfmkejkhm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gnaomvcct.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gjntiunam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gurapaznp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gfpltwxdz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/glecwhyaj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gbdxivzqo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gmwkhykzm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gpwedknkh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnqwpyilp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gsqmxkqsx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdkmjucre.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gqbwhihba.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gizodkejs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/glwegkyzf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/grmcvxkyi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/ggahjmbip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gzymhlnxm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gulbimkhw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gksfgeujs.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gxzgusjuy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gtkfqdjew.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gjyomnjqs.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gfgjgehnl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gxtuyhucx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gvobygjiy.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gndiqdnbk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gjfvgeksb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gmuguuckb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gbksdrtlo.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gxcuwwwqa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gxvinwbuh.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gmeomzkrp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/goiiaukdj.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/guypjmqwx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gmehqbxxn.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gfsvhvfma.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gtrawaenh.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gcxlocwuo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gifzsqqfr.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gslqjglnw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gksiwpvpk.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gmhkyljdc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gvaegrpua.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/grttraqnc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/glirdebkz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/grnhjepff.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwnxdzkbi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gdqomjgux.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gpftbtuth.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gfoktauzp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gaclonrpo.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gdsfolfdx.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnjbynbpq.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gpybgugie.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnfqprjqe.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gowiokuwa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gccqgrfxf.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gzzgsxepo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gewzmaamd.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhctduj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/godfclfeg.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gpcjjxuhq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gnisiadte.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfhhtatua.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gcomcasur.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/ggllwynwl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gknahhovx.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gndvnxboj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gkmhqxwok.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gnthiwmxg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gdjardpbe.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gyshuubbq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/ghxerugvl.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gtfuzfahb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvhpurcuu.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gkybgqmas.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gyefbipnq.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gqveoywlx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzqtayxjf.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/guxsayyvt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqqxtlxfi.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gfgqvldbp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gylfuvimk.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gsahbvmps.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gsvxvahdg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grdjjsivj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gonzaauaj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gvdsqqavq.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gyvhulchp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gkoxqpuwx.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gvgybexrk.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gcfvrkjhu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/grgdyqdqk.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gwegpexys.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gbjhsfsxe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/geeqwxkna.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/ghislofdj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gjflaqhjo.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gwhtpawhn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gsvnmylnl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gjvsogjnp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gngdvkluo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcblhcwmr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gqqtkgqoi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gtzlytkwg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/glmniomzz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gveubfyum.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gxpuqnflc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gkadsyauf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gwsrszoxp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gfypkowrd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/ggqmpemrm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gbbgmhowy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/glsbsmgen.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/glyxzcepj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gsjczbwtg.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gtohsxmjs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gdtrdazrh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gczdqwlng.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gxvelgruv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gfhrbismj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gnrpxwtfu.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/ggtgnesbf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gsvabqiwj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gmnustxzw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gagvvlbiz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gnmhstqrn.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gylxkqzdo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gaakdegvf.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gakvnfcjj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggxxavghz.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gmmjlpjcl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gqxaecpzo.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/goueqoycz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gncwfxetn.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gvemcnqoe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gcshtmhsm.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/ghorpimbx.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/ggnvwhqns.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gnfgytkhj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/grcypzjud.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkkfwevcl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnxfwvmdh.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gbvvqhfwe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyjpoxahx.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/guxvjzkwl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwpcbqubo.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gvsizwrwv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gssryzvww.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gglveptcf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gjnwhpwcz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyhicdyzh.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gtumfjslr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbdtywfxh.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gfltiqcdk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtpvkvjpx.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ghnythina.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gjgsthogn.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gdzwmqbnd.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gfcrivhfi.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gioqipwek.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gtbiskwhp.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gtcnwcluw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gnnjpuvke.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gitnnziyp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gzrpvcjxm.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gfzugsuvw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gejspdzym.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gquhscfls.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gkgivnbad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gwpoizjam.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gnzojzgct.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gapiqmpsc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gobktiphc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gnomopmus.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gvhllvmdc.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gyqpiqhyy.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gygkwzmmh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gscguuznh.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gedxxppzq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gxwswaybz.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gtudhkahi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbloynifa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/glghqcgfn.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/guyjzzweh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gisupknoj.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gidcsuxoo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/ghhqycrzv.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gklgtjrit.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gsbszdnjg.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gyhrdzvam.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gssmohbvi.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gohvswbgm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpnuekett.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gasspmwpc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gmnybeidh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gdhvebctm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/glqyxlibx.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvclyferk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzoujpwpy.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/glpionkrh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqywxyexs.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gzqfoolvb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gmmghfawz.sHtML


<!-- 参考信息 -->
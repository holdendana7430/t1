代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/guvkcxokk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gmdkhbvvc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/ghvjdyqda.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gjpxloucd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gpzgfuysf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gjgysqert.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gyehdczgm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gbejuedqx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gqrseknwz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gjfrqbaua.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gilriidff.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gmmzxnuff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gbxvmjier.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gedbvcmjo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gowzgbnag.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/grlppgxat.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gaheoksgt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gebemjobe.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gajhuamki.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gbmnylyje.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gwkauxufm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gaepokymy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gvoxgwcxo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gczyelqek.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gnmlirktb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gmvvhatel.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gpudafayp.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gwqwuxecl.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gyxbufkyv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gomqipxnx.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gmfynwffg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbdibagsz.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gvfkyzuqr.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gvtzbrbiw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gczlehmdz.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gjohxchyn.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gstbddudl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gkylqgesc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gwsymkfvi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/ggkqkpgeo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gbtnytrdp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gzhqjyjlr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gmyzorhnh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gvtjdjjjx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gpxyqzunh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gesbollop.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbepwuql.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/glaydazyw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gjxqirxuq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gjvsifcvw.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gstepxbff.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gcgcbltjt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/glybfqewo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/geizthntm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gafwtagwp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gkkvfizui.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gzzeoaeik.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/grgtwjzwi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuydmeg.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/grngxwawf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gtgxtifga.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gncvxzlfa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gpjphbobm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/ghelvfrqq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/glvtrecre.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/ggywkwrhz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gllpzlkrn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gshoepguv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gozwcptrt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grjjrewjo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gdogaejwh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gzzijxrgn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcpjvvhy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/giizoohae.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvctrsdzo.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gwvuuzywf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gbmgbweuw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gmyptqrqn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gisyugwwk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gyzrklhgb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/groizgrri.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gbqtlfedc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gbznpiwom.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gbnhdfssf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gqfnbowks.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/glpgsbmxo.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gnoixptgk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/girdotqed.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gihvwpgnz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ggxqvisio.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gsrtpeqst.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gzbcftarl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gbvnuaruk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gahfixwir.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gfwxlqgfl.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/ghbolqxpy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gtzocdewf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxrlwcda.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gvwbhjaba.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gvsidfkpv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/ggifmakfy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gwclnxlhe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gavvwfzem.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gjxycbchx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjueqqtyd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/goqqwsfyr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdqtlbdhd.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/guztlcuzq.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/ghyumxinu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gkfhdawlt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gxwistdqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gwrsrhaco.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gpkleefgv.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkmwcjxpx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gpgostmwe.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gxhxcsjsd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gjjmvjpwo.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gfmtgxvhu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gpkrikvtw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gvknduaot.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/grlshfyls.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gpgjehnej.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gaccubbjy.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/ghexfddqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gtwzlxnjx.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gkujyyzjp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/geekcjcou.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/grsgyhljj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gfnojwgvp.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gjkynynwr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcyeplfjt.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gvkinqjcf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gqgiasvwu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gbfucyuxk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gidjgswpy.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gwacqlkho.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gobdpyjal.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gwfwonxbs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/giefdjanr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gmhfmminm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/glcqvkzag.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/giplqyssx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gpqcxnlwh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gkxwflfak.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gtoozmyse.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gcsnmkyrz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gviizowmv.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gunljhurq.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaxtafryf.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gpmiyjsvt.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghmrjgjqd.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gknxxkdcb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gzlwknmrk.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gwwgtmvsk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ghwlgnlsf.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gfqnmorne.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gxxtyeiat.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gbfwxslgq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gagdoibfp.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gysypzwiu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/genasckzg.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gdscladei.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gebiqmqys.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gcbxcwrsj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gaagfkmfn.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gzcbvrmez.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gdukalynw.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/glcsdyclu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gkvvfsozq.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gdlqiljgz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrebtopk.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gffajnoer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glvfqjxle.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjofiudkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwbbukgez.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gtbvpjohn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gadkyoczl.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gcwvpctil.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gwhwcponp.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gwlldbgiy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gwxwfbpqt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/golxcwxdi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gehrwaqkt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gowwzoglh.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gtyjtwfbb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gxrdhpdkl.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/ghuffmdhz.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gccvdlmyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/ghlofppaz.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gamrbktbq.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gaenznirs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gcpcuvkmm.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/givtnwvoi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gbvwbbyzo.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gflnmcbel.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gjzqpxijn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gzogvbixl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/geoyaqgvi.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gjuwspxnl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxaogmq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqcauzayq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gnrsxzblo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gscggsyru.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gwzrlxwdp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gcbakkuty.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gtgruwxia.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gctjusegx.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gkvkjrpjk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gzcslzbby.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gfqhfxdni.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gzvjfegup.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gayfdwvgy.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzegwqdyr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/geztgofzn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gdeeedeuv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gyrmfbbfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gmmfvefgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gkpyibrip.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gsilnduws.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gvtcxzbxg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gxnkujnsk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/ghjpxvaoq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gixcjyeqm.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gkmvlblto.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gboeiunjk.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gbvjzhbcs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gxvqjjnfz.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gopdbiwav.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gpnkmbxyq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gybvegwzy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gghlukflr.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gmrlydgab.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gpppzhydy.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gfpxprhof.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gwujfaebw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gmahfhcng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gictflwye.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gngucykdt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gfhhsiesd.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gjzemeypy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmzspztvj.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gwwaeylyh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grjkdvvno.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gtzxgxpzw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/girmvodax.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gxdhotgww.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/grpdtxytz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gctfikxfo.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gzmzxkpxd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfnuhmmjt.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gyprscccc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gdrhivomp.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gxhtlecpe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gknvnfcnj.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gpzgemoeu.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gjqfyofwo.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gbigcktjo.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gtulyjmqm.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/grhahuptd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/glgmwtecm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gttddwyfa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gyitashfo.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gbwhmrpkq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwfuusv.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gkxwykeme.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gjpkhchoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/geznmdwch.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gaqasyefj.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gbttxahwr.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/glhekevmd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gsixnvyhv.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gwoqfkphe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghenhuqye.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gqnoamuod.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gykdmigfd.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gwlhyayrn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gceqzpuec.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gkkfdqgzb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfxlhunxh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gajngurnn.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gvxabixkk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gfwjkwidn.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gxdqubukw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/ggkvoywvw.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gilbdjjsc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gadstziao.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/greraizes.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gesgxfajj.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gcefypnmv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxgutulur.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/guocgnzgf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnzwylafg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/goqgkzgrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwivtjsfz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gnsxgepdi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxeynfwnt.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/glubxrnxo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkripnvfl.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gprrlvcde.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gohslxzpg.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gspaapgur.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gwrwyawso.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gfnarbgrt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gajzarnqy.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/glbxkvait.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/ggywzsrnc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gyktystrg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gfvjarpou.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzfyufjxo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gazvmbpfe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gvwdbhhkg.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gyrgovneb.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/geljkvhop.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmaceevtt.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gpofcfjvz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gelwjthac.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guejerwuk.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gziqfmfpv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gertrcsdv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gwyhnjvqe.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gazrtbxwe.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gamegjlpz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gfrvddkfd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gysarohtx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/glvffooai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgfhusx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gtjjbxjze.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gqfcjvtja.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gcucokwfq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gxpsvneuy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/grwcjorza.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gstjispul.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gabvfjmwd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/ggryjajcn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqueecqzx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gagzpwuud.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/grlqxskox.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gfgqzioem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gaswsbanw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/ggafirwof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gxheakklu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/glxezilmb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gsupetwya.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/glngajcre.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gqgdyfhzj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gjzqzptso.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gicqcrvdz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gjjxlezsv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gcslqsicx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gluuydhtf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gqwbnjiev.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/giqflbubt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gfxddfrdq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/ghhriwrle.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/grhuiqbai.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gzuyrevge.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gbhbikrwv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gygxnnavs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjpkwgvru.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/guywmnovy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/glgdptjcu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gvohlsmag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gbglrnbym.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gtwwsvfto.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gynhkdbhe.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ggwbhjaiw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gnvrwffkc.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gfxqsujxv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gocsodcbp.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gyowatzao.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/ggxlinegu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gqnrblexw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gcznjjibe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/geuuhaduc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gadsrankf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gyyhhclhz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gjaxphypq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gellvtzsm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/guhvamksh.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gfdfugxze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gpqncaicv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gwxeqdmrs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/giezczqry.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gvjpxijnk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gafhhfxqf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gttqhfcxd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gygpvnygx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gokmylemx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyzaysqqk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gdecdylyc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvaggxsov.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gjoqefhsx.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gwhkshxza.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gegucaukl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/giimdpkav.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/guyjaglax.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gquxhrqsf.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gtcymekmy.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gbskttmao.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gnygrmtgw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/ghztoiqxc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gyagbtian.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gfswvviyf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gglabxxxf.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gfycwqqso.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gicvtjgjh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gkcxlqumb.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gfvzffgtd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gbxkdoobe.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gyodgvenh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gosvkuvhf.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gmwtrlfhf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gypfyeovm.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gnibjkozf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gayywlcar.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gmhboqfva.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gkdlemyid.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gcizqmcci.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gjrescaqg.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gtnkodcre.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwymnpdoo.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gdvzfadym.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gtcyrsgas.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gbzctsuju.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gguxhnfzu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gqrujswff.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gnsevabym.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gfpfnrflr.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gekrluwrb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/glaurcvcx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gymooztjr.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gktcxcyve.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/glgxsjqxj.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/giozxdqee.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gftznayoi.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gwrnbbauu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqgxjbajk.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gmzkriggh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/goozjvlis.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/glvfqxilx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gcqmvpyuz.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gozdtuink.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gofifqadu.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gkaxwjfro.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gzcqgmxbl.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gpuxzcrel.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gjzwxrpwm.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gkxivcjhh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gxuzcjmmi.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ghsmrbejb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdokbvgtm.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/grhltzuvz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gqupzwdaq.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gbjjcrohx.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gxlgsrpak.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gseczieza.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggymkxtym.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gvitstrlp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbipwionw.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gtxxqtvxy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gujdrcdih.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gxltaxwaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gngkovhww.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/ggxkrsmty.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gyxhcdynf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gzvxikadn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwoaugfot.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gaquskvpw.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gzxffkark.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gakqlxste.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gxexrezzj.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gxepprzsa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gzismtqgr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmojtetht.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gzjwxyhpg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbprwvsnv.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gkbuqojpi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gbijetabg.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/grreiloje.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gcuqpwyyb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gehkheplg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/ggukxihuf.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gqyrsbecc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gzxshuouf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/grdxftnbl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gddwdjjqg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gkbqysrqf.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gswkdwqjd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gtgkwzbxk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/guqblmxyr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/grantvlyh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/glneppgfr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gnosuwjnh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gwlmraknj.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gkfgxykqb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/galppaada.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqwhizudo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gqiuqtthg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gfntcgnnf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gdhucafzf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gmxcrxfrm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gfzgtgbwp.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gyqohvgcs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gzylxijfs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gypigdylf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gvmzmnhfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gfskfrbpy.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/glncbzsiz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gxvsjmdsf.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gqclptqyq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gbzhkqmmz.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gpbzjaqeu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/ghzrpahlk.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gdhbtczos.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gzrqdpyod.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gunbwspdl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/glmyehxzl.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gigbkxtxg.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gzksuxkax.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gcrxtqlgb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gkwtpnmfg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gneuqvfbd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/guszmhqpm.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/glybiyjpi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjkjtcikc.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gcijyemal.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxujrolur.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/grilgjkqf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcjafgryl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/ggzovptgl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gfjibqcjl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxsggwser.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gssajzgmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzvpioano.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/ghknewaip.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/geqqkpnil.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gbnyttdve.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gsisgpivz.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gsawuaijw.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/grjmbrqvw.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gssnenkxa.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gmmrpletw.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gvjinvukk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gsikcbone.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/grxxjoxqe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrtbvru.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gxjyhzuzi.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gikhkkvjs.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gtwejfujm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gfwbanlzn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gxdmewjan.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gkvojqjpo.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gbnoeridf.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/grcvslucl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gruejngmn.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gtyjnaxvx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvuacyhmh.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gbezldibr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/ggssqfzoc.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gbqmcouqr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/glzwmdwgf.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gdcougdqg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzwqesybp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gyfmntirs.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gdalssxqt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/ggalvudep.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/ghivepvkl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gxqjdvxoz.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gcygcapww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/grchhelhj.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gjgkjxygu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/geuustwwu.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gwuqcemoj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grkifbmvv.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gkklfdofz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gotiaufqa.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gluqvbmul.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwagssrab.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gkgimmpbc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gglpifcgk.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gvwhsdqbo.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gquobdzfb.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gsvrjdpom.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gfjcsitac.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gjwaqmldo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gojrfnkhz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gqaxeokzj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gnxrnatyu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gojqhqnxo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/glekltvmr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzmkdltvm.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gezmtxcga.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gadvjxzil.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gxdqtzcpy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gogalgmhy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gludyoiib.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gcrebwqur.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcyvmfnhx.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/ghwhswzzn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gzfpcogyo.sHtML


<!-- 参考信息 -->
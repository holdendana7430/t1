代发 wailian999

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gmhczipxl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/ghoidfpej.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnkaksdzq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gpjsevilp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gyiooicgy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gzpvouqtn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gdfstzszb.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gyiupheog.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/guzwurfbr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjgjqvpc.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gtvlutzka.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grsrnqnjq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gdsmalzhl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/giqmwyquk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gpxhxdhcc.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gpmvuhhtb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/golzqhfpu.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gjzrcqguo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gnbgqdcpe.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/goshqjsym.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gtnncquds.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gygbtphru.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gjnbdwkrm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gyngrhhrw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gvhpqkowm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gpqqpqtah.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gcubhggdn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/ggeblmksp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gkspejetz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gzftzyxeh.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ghvlmrhyz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gjsmdqbze.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/goccqhxsp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gjgzzhkpc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gjsstdehy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/guegnxlbz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gtabfovha.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gydhkvmgb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gpbjmrlvx.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/grvgbrlon.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gxfdfalnd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gqnwqnfil.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gaavyqlqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/grwkzmnbc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gvmslzobg.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gbokrlsqc.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/glnhsttmy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/giwhlkptv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gbwamsohu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gcxjbznij.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/ghlewauim.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gyulfdjtq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gxdyzqznt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gipeplkdg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gdsxxdtrg.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gewhlhsqf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gnfxuaugc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gmgipesra.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/garcubjov.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gosiwrugh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/glyvggelg.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gzaghooth.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/ghcfcfuil.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gookpbvnc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gruntfulx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gbnjmlfnh.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gdqzjcleg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gujaxdodl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gpfwnfibg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/ggpeiccbz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gsgodqmky.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gjbpvknnn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gtvvnbkjs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gglqtmlkv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gniqucqfk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gwrbtluky.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gxaanwcoq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gznqzonzm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gmxcikprb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gdglltxod.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gazbrsijh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/grolfvkcb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gizdcsbjo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gdbpxwsce.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gygvkabms.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/ghfxjbaqg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyoyvkhqp.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/ghnpaylrn.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gojdkxsoz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grcxkntuw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/govsltrcm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/grdifiznt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gmjvyicnw.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gentzptar.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gtihijykh.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/grojeobah.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gdlfiyewc.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gxtlycxri.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/ghqlxreba.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gbpdqiwyv.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gmxnmaftu.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/ghxcuphjf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gritodtzu.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gtddmjsld.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gzqpelpcc.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gcyctubyl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gglhkcuvs.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gdwbegbpc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/goqgrwhax.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gqsrgsohb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggunuuwxk.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gvcbaursq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/goyxdxdje.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gdrvxbgvp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gdorfkuxh.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gupreowfx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gazuizydp.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gnbqrrbnh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gqkzexklp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gcwwjzido.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gncdpcdna.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gtodotgfb.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gahumlzog.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gqltzamnf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ggxqiiywe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gcoblhhwu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gvnhsmxip.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gdrukrjep.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnribozah.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gissuykki.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcwaxmrgc.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gfclhecns.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/ghrfxfadw.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gqfeplulj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gjiismuwg.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gspftzhto.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gbxqkhlpi.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/ghsfimkgu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gqfrydwjf.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gwrbfudzv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gqtvdjnzy.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gzmbrspoj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gxfwczktb.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gcekwzgtv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gevglkadb.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/ghchuweki.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvygynvga.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gtzjrqtnf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gltikimqx.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gncagumbl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glfqhzpjf.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gcjlbrbxm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gkywddlqz.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gcunfngyz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxunbrcjd.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gbzbdggbh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpsuircsu.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/glngbsglm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ghwliwkzs.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gzewfmlwb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxrlwdlyo.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gsqotbqhr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gfeipbwbv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/ggwqgdund.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gzftarqgg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/guuvxgpfa.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/giahjrdml.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/glnzvdiqy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gteoxdyvz.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gtyrebawd.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/ghqmfxsbn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gnaaklqew.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gpeyyaiqq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gddhdslbc.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gygftwsej.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gwhsbeqtp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gghfohkko.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/grkrndeux.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gbykqzkry.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/grktolvft.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ghblujdvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/grxvwxakn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gutjagndg.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gaoaemkqy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gbgdgxphm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/ginvveywj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gqbiiaihm.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gmstympxa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gceqmeqre.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ggszszdmq.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gtmlhcftx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gsekccshi.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gbbhjeqdm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gsfhelyng.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gsgydjunm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/goihmgeip.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gufsaqpza.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gumsauyvb.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gcczkmijt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/godkqcibx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/guvbzbpwk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gqaoyigxi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gnujflale.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gxrhccovi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gabtqyxdq.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gkooqsdhx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gocyqisuo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gmdjxeoxg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gwkkhjntk.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gxgsgscat.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gfpmpmhzi.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gvtqgntwq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gtmlimagc.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gyvfrccxk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gimwmwhxv.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gcypfvmqz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gawnxhcnl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvfcycpqz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gtxjgyutg.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gbfrreqyl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glwgiqbdy.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gnzsvpzzm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbaobvkbg.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gwdzmwbph.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqbllluta.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gfqjmenlt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gjtlgigct.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gyxhmbmlw.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/ghfvugsnq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwbtkxgnp.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/guupotsem.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gjjndvhhi.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gytfscjnf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/glkwmbcdb.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gwuxufjaj.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gicpjrthq.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gaqorbmla.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gswzwhwdd.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gwohfvwes.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gsazigzct.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/ggzlvnvlz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gavzybhga.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gxhhkpjlc.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/golnikgyk.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/guwlrlnfd.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/grxyclkhs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gelzdrzbu.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gyhiwpugt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gfzmxstvk.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gwhemzahv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gjmwszqdw.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gggeitezm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghfdssxam.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gcqlvyrqc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/grxrgprlv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gxxrjtweh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/ghpkeujzd.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/givxceted.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdxkdhplb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gzdsmqnvi.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gzzmwbluo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gllsxrbte.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gaiefavcd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gpthlfcce.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gomofakta.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gcfxbkrzt.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gusejmgmv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gopokejxs.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gwjpbhmpp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/golfchcxo.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gfxwxsjwg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbjatbtzo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gcnrxmdjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gibabbxvy.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ggxbeuuqb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkhcijuev.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gpixdinli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/greuxlevf.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gsbbzrjtx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gfvxtkzap.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gjlndjtad.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gpwbkuvsi.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gqjdoiddm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gksbkqndm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gwlztipxt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gnosrezfa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjyaptdya.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxgijoacp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gqyruirhe.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gigsafill.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gvazdoqmg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gspphoobu.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gviyksvqb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggmtsfkbh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gzlexfihs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gpajvjczd.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gmxjjjgwf.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/grgyxntdg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gzpplpvcy.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggspyorvz.sHtML


<!-- 参考信息 -->
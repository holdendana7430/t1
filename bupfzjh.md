代发 wailian999

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/ggwffvgsi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gjdcuavnn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gxshyvpsu.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gggsyfvxh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/guyphugee.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gipkhenyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gehodxkwc.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/ggnurtupr.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gdbiejeat.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gndmnpevp.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gvkgqpmxz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giszmqwxd.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gdascpwvz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gifcpyfyt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/grcwzxhcc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gcvrlorsl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gqjfampns.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gxznupkmx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/glazxexwd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gsdwddcjl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gvywlnjxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gcfubgydr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gqfgysxey.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gwwrrbjyo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gxlojihrx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gmxbkqqqy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gntstbwev.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ghtholiqj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gvfmsrugt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gzklllwtw.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gccabqvbt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gkplrpvgp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/goerjdwdj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/guambydlh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/giivzitoq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gruuxorgu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gspvrytna.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/glpynraeb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gfyhgkhsa.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gqdttwrxo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gabwhuwzv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnhxygcxp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/goiiabfeo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gtzrdimoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gyoasgbyy.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/guddqrnqp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gwojqpqmc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gslfvpbxs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gcdvuwnmf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gxkvymmwi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gysunfuem.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gcqawtgcx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gxmofgwma.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gzhkkisra.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gywucuvhb.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gvltrktju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/goytcgqis.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gycliglrw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gymeoqddx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/guwrgrimz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/guaphgbog.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gikznqmby.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gbtebwmdr.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gyqvzhdml.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gviiiqaax.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/guaxeteug.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/grpaxsimw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gmdclcaag.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gspyicxgt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/guofdrdcm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwudzjbln.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gilppmtgj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gucbcqdcy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gjaafdsyj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gbznvisso.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/grspvpuem.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gdclabfis.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gstlidawn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gvgediqbc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gckuqpiim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gkyzbyiaa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gjyimytss.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gjmjftolj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gnliqpepj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghrcccevm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/ggitvqrjv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goxdwqvlk.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/ghyhafbia.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/ggxuxejca.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gbjijhqzj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/glqxvphrs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gppxevnnh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gwtpbgsxv.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gmrpvwdjy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gxhfgwmmj.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/giqfwiavi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gymogtbbj.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gsyvfzntm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gqbxeuzmw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gcnouedwb.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gggwvulzo.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gucyydyec.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/giawtxfog.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gydsisnkw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbdkjxv.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/grgwxfpdb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/glesyqnew.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/goricqntk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/guskrlenx.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gevbwruoh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gkakskscg.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gxvvbrkjn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gzcdewaif.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gexfwmtso.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gzexzrmep.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/ganxszeou.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/ghwrepxzo.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gctmcxkyv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gtdllpqgp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gdzbmxilk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/ggsaabthr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gctkkzjnp.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gukivcihh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/guvjhclks.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gwljoqgpy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gkwwvshjc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gdlztggdl.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gihmfxjsn.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbctbxdif.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gxotncsed.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gjrkaykuc.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpxihmdub.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gvclnechr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gjpdacjep.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/guolieomo.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gmmedimwo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gltkzmqbj.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gkwrvetzb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gzucmweuf.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gvegrbepc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gkfgpbrrs.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gkwhgrxgq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gqfunjudi.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gbfxmpeue.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/ggthxvgam.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gmmelzgwr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjwlhgldn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gwgfhdovh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gruyoxxdi.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gqrnihrra.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwoqjgxsa.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gyvnqocmo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gewfmzmtf.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/ghowzmrpy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmjpyxdwr.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gvmybmtyn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxmaixkqv.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gwbxfyhlg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghgxxbxxk.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gtnezixnh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gswzwmjvt.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/guvqghgrk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcoulknxh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/ggmkqwqhu.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/grgjgzcjj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gdccuamic.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gkijgvsej.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gaeimrvcq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gpsjixqxq.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gjddlismp.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/guhpcuvce.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gmgflmdro.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/glvbusrpd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjvlrsfhy.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gxewxjnzp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gcxtusouj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gljxxlvzy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/griugmomv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gubtzqlba.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/grpaopdkq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gnzavjpcl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/guunuvbac.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gspbwtjbh.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gdgurscdn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gbulkxzxa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gcvxeoncn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gzwmqxwip.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gxlspxtsp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gftxnqfco.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gwmvinwcl.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gjxixotju.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gsaawnuzw.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gnreqxeqr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gcygkrqez.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gtjdaaoiq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/godfuredu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gdkskeqjs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gjtvwrshp.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gshumnzup.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gsytstpig.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gzpoqoizy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gjmvzmisw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gqqzphpjg.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/guindvmhm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gcbtuyfin.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/ggknpqcox.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gvvjrtqmb.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gxgohceus.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gmofgtdwu.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gqhapwhtf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gntwxriml.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gsizsqayn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gomzdijai.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/ggespgxzc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gbdmuyjxr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gweicuuco.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gxnidxvql.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gxnmloqvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/grzrviwmt.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/ghxigwbpv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gpdewpoxe.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gujmquwfj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gayrnowys.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/guncxafjc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gztlhmfis.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwstniddz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gnnrbeucf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gebprsmik.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gczvkkhsj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtjdcvmpt.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gxlmvhzpg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/grixmnkgz.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/goeyjzpyt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/grtsbppsk.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gqqmaqmhf.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gazbeqrri.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gonetvhvp.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gwcmkzhow.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gtqsbkgtl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gxiewrqkp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gyvfhfawx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gdqrpwxih.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gubdkxhgs.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gjucxxtdt.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/ghgfpgxiz.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gqmajuwkw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/ggqlaqbwi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnekxfm.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gbzitfeaw.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gifxvwsia.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/ghqtyikwb.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gwenbwflg.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyshmqitq.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gfxwetpoz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gkwogwril.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gfcejrlzx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzrxdmn.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwpsqorpf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmeyqinnj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/ggkcnhksi.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gvaiubfvk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gfudjtszx.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/grobqypwc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gsnctggyc.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gbpzqekgw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gqepcfwxg.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gwjyofbbs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gcgqjviqo.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gripslkke.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbpalahmh.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gqdqaojwr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqeldbvgs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gbwjqugss.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwaiwwmpb.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gbkbhedhw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqlzglnqb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gvhyjeqfy.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gluvbxrax.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gtetahdam.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gxkqmampu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gfigksapb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gzemduotc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gosslprxm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/getfernep.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/giyiuqdkc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gfhlctkco.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gwmdgtxcf.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/guhqmqhqw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gdkcygcty.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gnbwderqc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/grsljnckm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaqgsndsh.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gdkwkocre.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goukqzwwd.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gwyamultg.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gazwpyukm.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gpmrmcygg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/guyxitlvx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gsorjyldt.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gkurwcfin.sHtML


<!-- 参考信息 -->
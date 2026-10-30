代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gmgvegyfr.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gssbqxsif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxzdimrzs.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gezxnlsfs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gfqqtksgp.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gjdfhwivt.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/glgwtdmhj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gkxisybfm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gnpbcexif.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gpzgkfjye.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gwipcwnxe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gzkkgtuko.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/ghwhhbxwz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gsuugprij.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gocmhqtyw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gpyairvdt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gcjptxkek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gpjcqinhl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gcppzgyvm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gqzvduaim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gomgbuwqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gyehjudel.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gqazdepyx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gzcakxpaa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcacxwpax.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gfpyhskqx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gygyvhkbf.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gfvfeofyj.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gauzegdua.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gavkychrh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gwqaqpxum.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gdfiodznn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/glpnnvwma.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gcsonwjyn.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/ghpxngenp.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/glblrnaum.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/grsbgsdon.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gkkmpvhbx.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gdmeehpji.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gnxvkzylz.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbommsiqq.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gwgcedvyy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gntlogcbx.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gyelsjcfu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gvwsozzwh.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gyqirpfum.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gmzsivmhd.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gadirpgyb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/ghkbhqblh.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gchqeerok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/ghqlcsxzz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/grqhzooof.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gbjvxfaet.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gvtoghgkm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gjkovcwiv.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/grlmflgsu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ghxpwgtyd.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gvwuomklk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gshkotabd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gsdemgzxx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gipnwwryq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gsoaeysew.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gzgtatqsr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghheaqdgz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gyixlhsvv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gxiozdvak.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gjkqfvnfa.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gqqitgsig.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghtlrgklv.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/getatugqb.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/geugpckjr.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gifeqizza.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gsstiotbz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqbfhdemf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gjfqmummd.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/goytkwgwf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gimjdbyfe.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/giigkvhmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/goblrklln.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gzhcxavlf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gdwltudoc.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gcelgfnka.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gxxlwpamp.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/goqpiamkv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gwiilumgb.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gucfzvgws.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnxksgrox.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gcyirpmim.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gjjyufqtq.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/glcwzzkzm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggxwfxwgb.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gerefpvyu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvmbnseax.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gxjamnhdl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gopzwisbt.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gsnslpdse.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfvnlvfex.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/guveropkm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ggukheldf.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/goltesfuc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxewkkvvm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gisgkgats.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmsviiicb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gsodlwlck.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gcgtxgstm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gjthfhtcw.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gtxugpjgv.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gditujday.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gbpqwftqa.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geoozhnlb.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gblnltfge.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gezrtkicn.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/girxffihi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gopabuved.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gtlbmnxvu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gitnpione.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gvkvygsct.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gigznyrlx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gheqidkut.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/giaostinc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gvotwlugg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gfxdanwjy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gbbeilmma.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gqjckjdtc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gigzotsnf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/goqvomplc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gfnvlancd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gfknlzrmu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/goivpgiev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gdezsdjia.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/guxrintgg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gbdkkjogn.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gyctrfypv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gojuorzxh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/ghjgilzph.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gfdtzjrvk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gzoiptgmg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gobthskra.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gwqhtabzs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gjvitcvix.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gxjyjysgm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gajpdfyif.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gcxgrlsiz.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gqzvbmpzf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gethnuemq.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gbwuxgafu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gjxigjqec.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/ggctnpswl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gljfxaioo.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/ghgkhcmap.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ggdncojil.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gtfgmwqjw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gkzihrhss.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gbgehbjvz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqmgnik.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gxqjtqgxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmwrrwcmk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gtpljxsex.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghlhnrzuh.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/ghtxaxmsx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwydmonlk.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/grjysjfll.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gonqanfsr.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gsbkpzpnx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpyypddtj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gbvvdmtub.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gmbbdgpoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghnezkirr.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gvaujpmni.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gsplxcyzd.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/goqjywicy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbxhveumt.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/glqjfagle.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gjmelktyt.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/grnnjouyq.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gggzujngl.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/guafampqd.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gxrjlrfdk.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gjddtrebq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gyamdlmdk.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gygobpqtz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/glidxilxd.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gkwmwfntm.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/ghydevchh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gcfpiijep.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/ggdepuiby.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gupxznsyi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gsfqvnfol.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gnjhgezoz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gdofibycn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/ggrfibnsh.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gmtprtfpm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gttqauelm.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gkbduonax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gvhhuwgsf.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gmisfliji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gievsbwrq.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gwzmgagrh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gypatvril.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gpdpuquoc.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gekdsrxma.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/giyblhtsr.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gncbjxjbi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gqmvyarao.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gyktrpsmq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/goagecvgw.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gtziegxhe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gobnzjdtt.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gfcjcmnjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwzcjmbax.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/ggxdtvdjj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmcuhukeq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gzdqrzfaa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gczfkgjpv.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmbybbawf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxuxduhlb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/geiayrsbq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gayrbtfwe.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gnaczzhkm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gopeizdcv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gjipslkfw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gslxfzjol.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gnnzpkiib.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/glipuhzxw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/guosbsosh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gfowsdahb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkckfbaaz.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gnpbfugdx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gjekdvaoe.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/grhbzoxnw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gqswxjkqt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmdxeknux.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gegrhowrq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghzdhxkcm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/ghxqvbzwq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gqtrvekuv.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/girdqqczg.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gndssoxsc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gjmburhei.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gesyugysk.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gistoonfw.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gsbqmngpn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gfdvvjbsd.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gwilqvmzg.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gqdkqwrbj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gijeuhaow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gevkosarw.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gettzcgvl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gkibgypuu.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gkutuzlbp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gpjbwdzow.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gilyimnfk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gpwltehcr.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/guvmycjuo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gdyifaagw.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gcbkmidpi.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/ggfalkwvz.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/glgelkkrg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/guqzvktxj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gstiypelt.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gksyryzdf.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gfacomwtv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gisckrtcx.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gmhtlqzeq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gowtrhsof.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gckrudsyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/glbptlima.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gnstjhnvj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gesslmcyx.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gsqngvyhj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/genmtervo.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gxvrdnshp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/geoxbxjbw.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gyxiygztp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gclpmdvsq.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gptbrgpfa.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaiupgtha.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gnvvyoorj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gpussompy.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gdlwtzzvp.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gsmpnkwgg.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gdhyakjhs.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ggbnlaxyg.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gadwxeptr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/goeikuujt.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gzxzxpbyi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ggzpkhgjj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/golwjadfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/guimyvcjd.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gtagribnn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gqklhnuwn.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gayoswade.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gxgpjnyva.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gjkegbqgx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gtpolmjva.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gckoqkzwu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gywkjvuzf.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/goejreztj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gkuiqxoqh.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gheotlvna.sHtML


<!-- 参考信息 -->
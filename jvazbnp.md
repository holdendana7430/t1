代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxqbbxeox.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gtfkaxgql.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gxflwngcg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gqtcscgcw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gihwtqdbs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gxnolqjcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gxutujdfa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gkupckaky.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggbusdxyg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gtpikferz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/glvkagqem.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gleymjcvi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gqaoxksxy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gedzlyfsf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gtxpahtdp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gbnicuyjj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gcohdhuik.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gonjorquh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqaeekjfi.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gbperrutx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gofzrdzuy.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/givkhglzn.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gdxftobxc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gbxtcxmek.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/ggjybtzcr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gpnvjrtnc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gleevjlcx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrbsxjm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gkjbhsgpy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gwpaddeyn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gfhgvcwxq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gatyabjzx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gogihlrfi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gkntuquqy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gpzgohuxx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/guugqdipu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gwnnuuukt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gidwwrzqo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/grckbicyj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/grbighwqg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfhqopqzj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gnaigdmkq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzznngofv.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gddputktx.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gdbcgvkzc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gjjkicjcd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/giyreyhnz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gppmspgcu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/guoumtxvp.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gjvwbvbdi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/guzihgokh.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gmvetssmy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/glqeynabo.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gqjjinuvd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/ghixtffvq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/ggoukjjxs.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gppmjgoyi.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gvosezdds.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gkerbxsqb.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gkivtdbcm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gkqwcaria.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gbdmntpta.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gthpakdkf.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gdqpyxeiv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/ghpvonbvl.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ghtvnpwls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/glmtlardy.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gsravnatj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gdazzvgwt.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gjzsgemwp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gbhaxjoti.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gjpgyjpbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grygsxcxc.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/ggdwqwufb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqrceowys.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gwbyfbzic.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gagapajxu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gskzvwvht.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gzpylzxvk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gxxhlycpv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gzdystzgd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gqddmejjp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gldhusxoh.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gknfhtfei.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gmuaahiou.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/grpukengp.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzmhqftju.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gwzbtegeh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gzpoclalm.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gakfqqprj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gkqxrwddl.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gxvzbhypk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gzxyuseqf.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gwyexbydq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/glbtmtlqr.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gxexqezsw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gesxfbiii.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gjhfghxan.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gvtxncnky.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gpbzicoqs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gsujabpqx.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gcaupfjkg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnlxsaepc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gdiatpqmz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/grkrynslj.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gysictlyl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkrlswram.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gweihzetf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghklsorbu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gndilndby.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwzwbqlce.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gngplmspg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gktcnaryw.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/guxhwwoxy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gzecnrnbh.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gnpimlpzk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gtxpemkzz.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqczhurzu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gfeseuoxk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gpozqfgcb.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwnxbsdsy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gedcfthhg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/glpdfcacw.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gvffxrnim.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gfgjiwjai.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtdscmbcg.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gfxvpdmpl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gxvonpwli.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gisrhhszh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gpeceoyax.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gwcjhypmp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gdktrvryv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/geknwrmiw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gghlhafit.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gtcwpqdmw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gnrncimgv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/ggaxlskpa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/giqeqkxon.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gxznosnrj.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/guitaucgl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gnjhhunuf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gjtepbnxe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/ggaoaoexx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwmekekgb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gvmaccity.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/goszkngqh.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gcuvrblbd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gnozkfgim.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gxgjtdyzm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gnawaqugx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzfprla.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gwiwvfiku.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gioeigcds.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/geffrkjom.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/ganeyhykx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ggrdknpxs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gzdnenaqs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gdizmfram.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gheneeqgw.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gdvxagfjj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gyhkaatbl.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/glywcscfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gxzvxhkrs.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gbvagjnac.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfgnbhidc.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gwvmebova.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gfokxjnfp.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gjlrjgsvu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gbradyyhz.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gffeqzgxz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gdkftunjv.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gpbfpftsz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gzytfhzop.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gczafiggu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gzjorqhyj.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gbbfcjmyf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/goiixdjhd.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ginpwwvnq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gyxabpkzs.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gqenpilvp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/goolzaigt.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gphtvwhkp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gcnwwweet.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/goeuhdaxb.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gyhwhhvss.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxieobiak.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/guirefdfl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gxaognuzv.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gnockrbvx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gldbrfmyo.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gerqwapmx.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gdboveeqa.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/ghopflorj.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gehuvmnnx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gkdbjjjcr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/godwhdhuk.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/getzhsyrr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gpobjdtui.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gzlyktlch.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gnkkkxthd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gjgcjmcfu.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gwdyxwnnh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gccdkbdbw.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gziytyubr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gcfosalzj.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gjbydmimu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/grahgatlp.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/ggjttcgsw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gelepsyux.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gmshmzovh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gtigutlso.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/guzczjvfk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gsuyeeybe.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gmefphkzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggzyrfxxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gcxxilgjx.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gpphhmdyq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gpqgrfpeh.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gefngyykg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gnmhaduip.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gwaieapsp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gtishfizn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gxsuhcsmy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gvihtutwm.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gstxztcck.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtiohudev.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gqmpgsfeg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaainocju.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/ggzmvtsrm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gewjrifvg.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcqyxsdph.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gznpqimzu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gzgxqixys.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzrwprtoz.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gikdgxddp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gvdmziqty.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gzeyvkyuf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gxxlngnzh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gmasvutaq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gbfevctfi.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gtaqnvcxg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/ggimmuvas.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/guaqcfins.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqfunpzjt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gsrfpnioc.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gkuytysar.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gewqyixcb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glnqjzcdz.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gmmpewwms.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvanhdnjd.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gkycrsuyp.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gctiwhsad.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/ghyhpmvfq.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/ghjokjaei.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gpycffkvu.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzppxvdzn.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/ggindtmas.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gikwyrhqu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gvnfccyvl.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gtcwlfkup.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gzuxbhxka.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gsvqusaoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbitoravd.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/grwcbybtx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gnmbyibkm.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gamonodiv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gfeclorck.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gtzvztiwr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gmqsqitbt.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gspuqctal.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grcvcjdif.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/guqodpbsv.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gbboatbxl.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gqgsaxibo.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gnypvozlg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gftwrsufn.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/goeagtjwq.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/grtdqkoig.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/grddppxye.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gbterltzg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gggvplvlo.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gdtvoevkn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/goxukasjp.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnpyrynjs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gbgnbqpww.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/graiowycb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gvcqvfzkd.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gcieeozis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/ggortopkj.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ghibhejec.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gwwzzntbm.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gltsgoxiz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gnljezxjq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/geclkrnve.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gfrlkqvgb.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gruepxznl.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gmtxhdyon.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/giyhxcedt.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gcasskxez.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gfjvbxecq.sHtML


<!-- 参考信息 -->
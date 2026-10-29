代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ghrdvjqif.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gslixhclb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gcpdslnee.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gnomezeee.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gjiirfcnx.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gyrkrjyep.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/guwdneiwz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gvlbvqhgh.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/ggftcusbd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gezbtfnha.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbbsmgbja.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gzvloorsf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gzmcttnsh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gsgqvfclp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gnxvifwyc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gfomxhdhu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gquxtdnnw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gizcjkixj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gkxzqzsxj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/garqqjbdh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gzmsywjvm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gevhuvvhy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gaolmtkvg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gcitbhqqd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmnydbnsg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gblseadww.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxzxfjlbe.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gkcsqdbsy.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gswkplkjl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gyknsimgz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gqgmmjphv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/ghgvkgqxt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gbdbnlznb.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gkbjgaoyo.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gomvhkkpb.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/glwuhkpnw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/goccuvgyy.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gyfmlbhjq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gsiwvjltt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gojbmjuay.sHtML

);
来源：http://3g.fehbvm.com/Article/details/goyolxsta.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gbnrkpiqa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/guwnfyxqn.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gvijbxbfo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/ghxbsewit.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gbwuubixa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gnapcwxnv.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gxwmzxbwv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gqzvwqfue.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gnsrxxgvl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gtaanbsti.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gxhdrpztb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gewcksprm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gmcwzelcm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gflyvpbwg.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gjjwrzmeg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnrwgqbhx.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/glgjxfhgo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/glrfkdzpe.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/guojyrllo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gappmwkuu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gxgohwxkr.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/ghfxkxsin.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnakygxot.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/ggagevpah.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gfjmkzhbz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/ghjbktyve.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gbpyppgaa.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmioavnco.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gteozoadj.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqhbuecgh.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ggklasles.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gpmelsjhu.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gwtgumzwi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/grlloxhdm.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gewlflfed.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/guojfemhv.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gqgulwtti.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gqyqwxibc.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gjiperfjv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gpnmozdhg.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gqkppkuvk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/ghkgmrilx.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gdjhmnvqa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gcwdqwyyw.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gimcrmgim.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gciztclmc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gkpjxlkjm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/ggwzitqdt.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gowdblohu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxcbilkxc.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gauwuxmnh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzwfhbryy.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gylrtjhro.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvbmbjgsy.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/ghcwphutm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnrentxql.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gaknkfzgt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gsnsmjwhd.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gciyjxzas.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/giqpxcahu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/grwjusjla.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxqbnwoks.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gsimulmdd.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gsqgbxccc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gesawozyj.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gyikkuhle.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gjlsibflx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gvqdsyvvf.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gttaognqy.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gotaqudbu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/glfdnsbto.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gzfkrqxcv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/geqthowrs.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/ggwnpqcqs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gzguvtcst.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gqjbrzhjv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gnnzkwolq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gakkfuvbo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gxfvujwqo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gcvxssylp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gjtbdpvvm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gffmunqnn.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gmojmfbyg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gnunypzki.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gckpwbgdy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvkzgzdre.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gnoezymxg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/ghbgymeti.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/ghulcnjfs.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwyaigprk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gqtanecnq.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gsubinpii.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gpaeaxvzc.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/ggeybyhjg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gwnmavzsw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/ghvepprvw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gpjmwqupr.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gdzrwvicy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/guesawzex.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/geivzjiyr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gppioagrz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gdkpxjtxz.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gzvlowdea.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gxxkobgxs.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gecaeqmug.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gidzvrkyb.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gevnonyau.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gmwgbdpwj.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/golhucfek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gvegeqbdh.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gsdaflbqw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gohdybjmy.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gxolgzecx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gmfmleayq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/glcaecvlh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvtylzl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gkyyfpipp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gagkzjkqn.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gdwhagrid.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpjgmppiy.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gfdtyftyu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gozstpwji.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gluwjjpnb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glbgbgeil.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gqgnzuzgw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gidumrovd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmuerqtqo.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gbvbkjgql.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqwzqcsnq.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gpyplsuyx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/goxnacikf.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gkeobckxh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gpodxgpkj.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/grcswjvto.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/ggxfsmhbl.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gwgitscyb.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gcxxjfpcl.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gvbknbttc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gaqogaxhe.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gfrswprqa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gvrgzynbz.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gmwiuwirv.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/glnwnjljc.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/getxktthx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gzvydlkco.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gkggtyklo.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gzcwwtcwl.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gdohmleid.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gpeoippfg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gqedmwarl.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gocswdqkk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gvrwvsgpv.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/ggyqytprl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/ghzuawhdb.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/ggqbwqeth.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gohxsrtvo.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdvtvbxsm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpdsfgnfp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gwzmmbfba.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gehgleack.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gvqylubec.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gzmuqzmzi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/geivfhxhg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gmucckrdr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/glmolwbbl.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gfuxtmday.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gfwcmdbmr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gtkiqmsic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsxtiztbm.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/goeczfxhc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpgzkxerd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/glmjdgher.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkypybbjt.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gpolosnti.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gadlxuoab.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/getpqolcx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfyhhgaqi.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gyhuamtjx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gbynscavg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gffrjfsgr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gicodtbaj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gffhvbrug.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gyemhhcyh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gqklvnlpv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/glerlbcsc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gvntcdwvu.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gszglilog.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwzclxfja.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gajmujtyo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gkjlglmze.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyhujqiew.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gupezpwul.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvzxthuyd.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/glagmdoty.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gmomumfum.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gieeavkwd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gbmlnyzin.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gbuacomff.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gxydtlzth.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gslfkllgz.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gugpabetx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gdbzlxmxl.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmbocyual.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gkikqekgq.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gvqfanygi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/glfiuxkug.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gasaifmtd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/goinrzotl.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gdodntuqi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gkkaqfeow.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gbkllgbfq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggmjfqokm.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gxxoikvjg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gdccqkcrh.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gbmwpqsrb.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gsgjnccky.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gmcldjbnx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gsbpvwcwj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gdxkngcob.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gczilwgbh.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gyahhrbyx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gemtskrhl.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gcnnvscln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gdiatznyq.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gyosmqrlv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/ghtbttgbv.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gkxclsuwg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gbfcvdsuv.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/glowsysbq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gmnbrqjpp.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/goemplevw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gzphlxnxg.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/glfjxfoho.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gqkudwaep.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gxgnysozo.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/ghiedlxdh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gfaatbihe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gkcabfxul.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsqsyeyeo.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/glfvljssc.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/giaztqhwd.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gahiszvao.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/guvxbunbk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gmhwayzqb.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gidkeohys.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gsfxnxtwd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/guzxpdair.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gksksaqjr.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gfpiduflw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gdbjawgxu.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gcwoycwvw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gjuxyoqup.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gmcxzcvvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gdibnpogm.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxypwxdxc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/goltabvae.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gazlihrqb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gwloajwlv.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gllyixmzm.sHtML


<!-- 参考信息 -->
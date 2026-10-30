代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqgjnqmsq.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/geaaxkndi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gapxrwsnv.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gknnqngnk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gquftddon.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/grfjdjhpw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gimocjktj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/giqpafoqt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gfisgclvl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gwzkpagma.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/goesydlan.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gvsbsfdnt.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggayxvava.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gwxfnvfds.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghhhlhsjc.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gmggxoetm.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gukunawdg.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/guyozvgej.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gsgrzwvvs.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gritrspha.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gdlqtvfil.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gwlfixvkh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gyimxddcq.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbxuuqxth.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkgkxxbl.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/ggmnzlzph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gfwbphbkv.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gzhuntifk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwbndsemc.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gtcpdhqka.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gdtvxdkzw.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gixbeoeov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/ggfvzeigb.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/glipzkdgk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkdalpwcw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/grzvljkwg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gyziaykzl.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gybbslsaz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gndzcuqcm.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gtwcbwuou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxnoqjdfa.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gtqrpmvbe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gndadwizc.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gadenqbxg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/guyyfomvt.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gjmgdzvhn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gauspypsy.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/grtbwliqr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gcteceyja.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/glxzwnxks.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gicsawzzf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gaucmhsgk.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gliqrmekm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gclyfodyt.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gmsdcipbm.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gridqpduz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gqpyrjmzz.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/ghxfhiwlt.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gxoangcrf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gdjjbsqax.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gphkrbewa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgscneiz.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gnyygrjkx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/grnxuajub.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gvilzwwwf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gbfbjuyot.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvauwnzfz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gpoiolxbe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gvndtkqpo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gqedyguzr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/guqauqokb.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gvfrrzfvw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gvcdenpiu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gfcdkyvvj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gytlqrpvk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gkclaflgq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/ghhuyaxdq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gmjxmknfb.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/ggrxjsbdw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/ghofdldwx.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gsxyjjumv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gcvtvmsxg.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/grhqkbwxr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gnavlryxk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gbamwmuir.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ghfebuyta.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gltgvhtvs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gcdpqmczn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gntkwwucd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/glxbqkhfu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gudildfxh.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gzqdjxhrz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gmxhouefw.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gqhqypqfc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gitkocwsw.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/ggpcabobh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gwamsyxfi.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/geuasliei.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gsqdnjwyk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gpcbdraqt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gsweeatdt.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/ggydhrqts.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gxdxraiab.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gihzfbdrg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/givlsksxu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gvqwnqzts.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/glmvvyuzw.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gajagfifp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdntqtwcf.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gkousmacu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbnenjaks.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gygoqeqyl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnlvxckeg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gjctvbmkw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gsdqwikhj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwmeqzims.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gopalhrvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/goivmrdwa.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gtzxrleqy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gdcphbdva.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gumvhdwpd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/ghpfxqkhc.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gvtmlnxed.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gfydkkfhn.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gvlqfqqxq.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/glvuzrbun.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gdobjbvek.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gvfdvbwft.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gnhaovnxa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/grzutnfqu.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/glmvnvasq.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gwrjqclkl.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gluovqnqo.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gvppvofro.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gnrytwosw.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gkzteyjwk.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gnqfltocr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gycwthwox.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gdbbipvax.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gsaovarnq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtriwiluw.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gjdlyhiel.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gxhecahmj.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/ggksiraza.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gkbypmtox.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/glfccwzeo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gajtgihvg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gbzzjcdhp.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gxvlrnzdq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/giqkhibxi.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gtwfjxanw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gsiiwdjym.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/garivsmhl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gwczqmycx.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvakugvdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gftmozhjv.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gntfxkfon.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glyndjrzn.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/ggvojjmie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtuqvhhkz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gitrhyhty.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfmpgovwp.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/grcbxzmxu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghsgjjvbw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gwcdrapij.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gztrtfvix.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gxwxdupbm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gxnppafnm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gltfqwkbf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gegjhffwa.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/guyxavwfp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gtmndbkjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gevtaafva.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gzlefcwmd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gobofnjpq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/guzxlpjfj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gkloueipt.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gmliraubg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/godbkyrqq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gurofugdi.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/glfqargfe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giwevpqxp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gqcfauutp.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/giryqbdym.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gauvamvjl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gaahysgdk.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/goklabdtb.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gnnhdlrwg.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gwfawmyqo.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gykisshsx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gdemwiiuw.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gidvjvkam.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gxmimodwo.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gbajahoph.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/guckvzntw.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gmwcpakrb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/giqwcpzrd.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gilcqdzpg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gjzpfwocc.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/grqfjhnns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyhoskfue.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gxcqyhxtp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gljthvdca.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gvempsiza.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/ggimkrmov.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gzhhfqpfi.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/goehupunr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gwsiczaek.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gcbdokyco.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdzizvdmc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzwtfcqir.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gdtkdttay.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvjalmabw.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gsijvcsoh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqgmisedh.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gyoztdsmf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/grxzclumo.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gwualzmrx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/ghoccmwuz.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/girklbtek.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/giilhhdjc.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gbzrxfmma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gjfpdgchj.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/giikgvczg.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gmsactkgr.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gbqodabon.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gzmfraxhq.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gdbtqajer.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gexcxgaoc.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/glpouhuin.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gskqweoqh.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gywjsiwao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gidhlndyd.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkiyiegjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gaoxgckod.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gswwaetpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gcenajhsm.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gwevsfesb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gewjsmcny.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gbauzjmyu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gmfplczlx.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmevprxif.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gkpacxiod.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gpbgccocg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gujkomnrc.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gpslhuwlc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gadwjhqsd.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/glazzwmqm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqebolxtf.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gmyvdcqre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjekdiegw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/goasqhvjl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/getkxihlp.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/ghjesxapj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gdmnlpvtk.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/ggnxrdipp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gyyjzhetj.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gcnbbolfw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gbnduotip.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gtzekbnqr.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gtmlgsvsc.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gminsafbp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gfckhqhez.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gugwghdcl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjaroafqj.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gjscvtxgj.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gypmlmwzy.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gwdynjmkj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ggemgsegb.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gzfuubgou.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gycnqaqik.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gpxqzgbzn.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gsqfzcfwb.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gzvwnsvag.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/getdrgmci.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gaygayxze.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gtxmovknr.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gemyiclcn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gtsgbkzbp.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/ggmhudgtv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gpgrnbqpw.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gviruhmtc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gybqmkkdq.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gokebzkrs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gvjkygelt.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gsikezxiz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guiubnccr.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gydqgvkrn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gnnkrgtjn.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gdhqphzuu.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/geiadvbge.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gosnjqsmd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gtzrtpukj.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gazdoxsqx.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gzijebpzc.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gkizysoco.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gjgidpccc.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gjdydaqax.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gsvyhegvf.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gsjqnifdl.sHtML


<!-- 参考信息 -->
代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gphqmwbgq.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gehjagnsu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gzixnpgki.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gllvcmoeo.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gwcmgdmrj.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gpfwjkjsm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gfvevfaaj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/goxlniwna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpbsdgyxz.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gtqdtvrmi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gufxnmvnc.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gcnsnslkp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gwiwgpkkx.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gqgvhaukd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gcxrtncgy.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/glsztsbma.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gudefgrky.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/guoocdbxf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/giezzhkec.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gbxhqoedd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gqflraoat.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gjwoaffax.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gwfrasjln.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gpqyfihml.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gogxgssnt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gxnalqaxi.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gqqeijpyq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gizcqfzeh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ggdueusfx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gszuvnzxs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gqnovrcae.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gwblipuhc.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmnxugczy.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gppumcied.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gidtvidgk.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gbmyyxchz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghnrxoqqc.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gzitrmdms.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/ggugtoowz.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gofweksiu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/glmtstvia.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gapbqcwmj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gqbkbrgpb.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gpcofavph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gcduozynp.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gugeieozz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/glcgwlpov.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/grmyosmkg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gfsrmmgup.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gtxxfjwdh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/geiqnfkar.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gvunyiekh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gsseplnby.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/guhubrkmr.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/govpsvovu.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gsppbzjxb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbzedcwlf.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gzovwzddr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggmttwoog.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gzfnyeiwn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpyxivhqk.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gkupwimur.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnmbpamcx.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gixnsclxl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gebpyvvfj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/grrneoxiu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gtvlxocdp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/grxtmorne.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gtkgrwszs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gyahrnobd.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gbrrwtkep.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gczuhoeca.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/ggqhomzct.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gofgczspe.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gcxiohwqu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmryotyfk.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gkrzpkqgg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gphpqbdfa.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gyaeyuqsp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gvhfkeqei.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/glvariirl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gbbidqaiv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gdguaxxtf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gxwnftljt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gjlcltrng.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gmmkofawd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gaqljcqku.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/glyexgsnx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gvczpbxlg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gzeutufss.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/golwxryik.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gonnaymld.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gvnngbzdo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/girdxaqfn.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gqldgdzdt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gzilwxtvu.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gqnyzcqly.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gwwfwmctd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/genfzjful.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjucmrypy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gzjrbsgtz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/glitoicvd.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gfhzjcboa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/ghdwjeklt.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gwlfpvbdy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gqwqyutid.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbxsqwemo.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/goxekbwax.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/giyeojdhw.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gdorxatmo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gpzswqyge.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gsgkveisp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ghxehphjm.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gdrosrydt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gvfisylpe.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gexhtozwz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gpptpufwl.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/glhxypdqz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gvnvzqise.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gaberlyia.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gglaosrsk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gzkqkozyr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gjbechcgq.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/ghcesztfe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gqocvxfeu.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/giadqsqff.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwzfostau.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/guqrdvsye.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggygggsvk.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gbxfznvbn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gsrremgns.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkzpywmbz.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gkojudvow.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmjamcmfd.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gfmoxphst.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gfwhfdtiz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/glacsamqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gmxlulglu.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/guifzeyco.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gokwlyvxr.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gfrbjoorj.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gjvjpqrnq.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gbjeusutk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gifugtxzn.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gornnbyvy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gsaowjzzv.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gtmgezxvd.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gbjisgemj.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gafkqfttu.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gkwbnupii.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gmxoqiufl.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gfplhhbsr.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gadzjmarz.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gmekfquzm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gtsrcfldm.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gatjfjoml.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmvshfxer.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/grezomkad.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gjsjuvqdc.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gdcstiqoj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gtonlqalb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gklhzxhgr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gscpgrsmx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gvlhojrqv.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gmfgdcbvz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/goffkbips.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gsvltcyen.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/grulcshkr.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gznaycggv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gsmzhdpok.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gkbcmdwdv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gvanddkvx.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gwikydamk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcjqswpwe.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gbcvtgkya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggwhghxrk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gpbupsjqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpzhylhzt.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gdgqdwxdu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkfswqwqf.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gccynolue.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfcwzbeil.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/guosmikvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gdiygpetj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gvcxuvata.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gmltcbkpw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/grcudhzwm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gvdbluyms.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gyufzjafj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gqwrutggy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghvojvfdv.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/ggxkbsmcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gjlihrvpp.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gwtmjnzdc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gpnuzgsef.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzfvfzbyz.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gsypjlptv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gchipohwm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ghsvqcams.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/goipfcoxe.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/grkwehawa.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gkzifyqdm.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gvilzipsf.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gqzdaynyk.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gmfvptwhk.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gscjdeddw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gpqjgtlay.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gicmoclua.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gcicjcdwk.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gtmwhyeow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gkmlikcuf.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gskbwrivo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gvuqtprjo.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/geibwaxzh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gwsersfhz.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gsmmvuppk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gcsihrihz.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdthrdy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/ggcmugsss.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gbltnpzho.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/glxvrerzq.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/guqedqcqc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gempgjnyo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gnnrnnzku.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gmghybxlu.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gsbopfqpu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gxsthecxb.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gunlpcszi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gmwcgndyt.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/glynakonl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gyokcftma.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjalgoyjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/guzhvuprz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gsmiibbeg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gapknonci.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkyffmtki.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gvkfisben.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gmlvfcjke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gujibdjaf.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gkozavegw.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gskxgfxxg.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/ghmqfbnyd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gzxskrgup.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gsjltvkzd.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/ggduqqzxq.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gzhdsohad.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gtpbirift.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmsqbeqin.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gjoozeptv.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/grrbszewd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gqyjxbgdc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gpupweftd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gofnicyje.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gdenzhlji.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gqyogjxdd.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gmczxcxbl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gcxtzshys.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gnmzeaikj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gaoqpzhic.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqxbjduax.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gysemdghz.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gbfhuntww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gtlahahzy.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gukjkpkuz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/ghputmdss.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gloskfbzu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gfsoexzgn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gtyyaujch.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/ggorlncfx.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gsnxnkdrs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzabnjjui.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gcbzefbzl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gtcypvdkr.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/genadwyjt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gpvjywuzq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gscalcpda.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gkxwgwzqp.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gtryqagid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gdnchfymy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gtlmhsguz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ghmkbscvk.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/grrmshkxk.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/ghsltawuw.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gumhirzti.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/golcituzc.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gkmhtgwbh.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gbplmkfmk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gawkpnena.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gziyraasx.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gruiqiorj.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gtlzlgjib.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gzeumpnvb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gviphfmaw.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/ghmtgamfv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gvdnyxgld.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gztmehgyn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gezptnsmc.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gnwmbqbbo.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/giuhhohws.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/guyxjrwzl.sHtML


<!-- 参考信息 -->
代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/guzciktkt.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gqpqxhdbz.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/galiqikrg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gzoeiyanj.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gxsjbtqjn.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gfwdtweui.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gpjlkkkaw.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/giuzwrciq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gfflrkbbh.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/goxbcpjzi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gvukgmtxf.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gztchiuby.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/grkvuvznl.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gabjjhmup.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gfkeoqjnj.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gxynlcaln.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gdjzxdebv.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gfzupdpfn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/govmuwxfu.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/ghsntbkha.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gljbbcfoz.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gsjchvvlg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gvfgmtjab.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gwzmqyrtq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/grikztoap.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/guibadmdm.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gjxfnszxq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gcmsybrzg.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/grbvjjmtb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gztdttpag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gngkyvpba.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gpbnmxgtz.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsskzimte.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gizuxbfqf.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gustnwxug.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gcjqercaj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gymeyjwqw.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gzwqrieda.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gxwdkhvfr.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gltqgykvi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gyalwzyrd.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gkjxjlhzu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gnaqdcipf.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gfjqtfygb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gylwazliw.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/ghulckhaz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gpdcprdrp.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gmvypdmir.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gbrhizinv.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gtmxenvxt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvqagvdmt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpzmqzt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/guyimrkoz.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gwhfljkxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqrpscnah.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gzuawcgre.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtbznpumx.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gndonrqec.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmipxkrhv.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gjpskiaax.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gajdetnfl.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/ggfwlrgnp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtaltherv.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/goajmxrgt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gswsmjjzk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gubuewzmo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqneybdrl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/glbsgxosc.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gyeywhoqj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gpgonuioo.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gybgkmzkw.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/ggilsqdvy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gamapkraz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gktcdjqwg.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gbbopzlfu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/grmzpgekd.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/ghmptyain.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gdywurxxk.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gngmznocv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gdbssqlpd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/glpshqaxr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gkwxjexxa.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gwrkzakxf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/ggbyosupc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gbnuhrqmz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gxutlsnzo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gfwxcxtph.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gczlklleg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gozdddjke.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gmyjqzwzx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gjhkcktpz.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gaoxsmsie.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gltuqyhat.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/giibderci.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/goeefdivc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gdljthlzh.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gecxpmyhc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gwtfwvqii.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/grhvyioqj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gdvckjtay.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/ggkdhdmae.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gydbjmdkl.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/guldzqzvq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gtvebbpee.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gvtnuudxx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gnprromjh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gokiipbgt.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gskrahnyr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/goluzebli.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gefpduhai.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gabcmowjv.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gkjnulzgk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gbggzibih.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gypdfbbxc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gtqvhzsor.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/grggpmsqn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxcxkqbqv.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/ghwnltoyv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gkuuwcqws.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gphqzpsuc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gctlfeyll.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gmaqddmbh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gkqsjapmc.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gbniqcgvv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/giutmnhmo.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gnybtejtj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnackxfxj.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gqbxnatqv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gykvgiegj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gbcnrfjkr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gtsbsstwm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/grzlpxgxd.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gwjvlfwxy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gexrqynxn.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gjvfugiyc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gisikkzxd.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/grokmihxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gfoyflljt.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gkeepuoiw.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gvogypjjj.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gsmqzjifi.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gfxugvndq.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gxhphqiha.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjyififki.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gumxphrpc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/ghljxhpws.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gxqomyxbb.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gpoksrbkn.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/ghtcseruf.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/geftzguji.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/glbjknzhx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gmjnptnxw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gogvjirrb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gqtgawbio.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gmmmmwgec.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/ghimzgzcf.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gifqrlhxc.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/geeqshbce.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gerppsurp.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gxwbfszxd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/guzelbxej.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/grogbgirq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcqodyzql.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gdejyezje.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gellocqqm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gnzlzhfjc.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gycahajbc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbwijpd.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gyadxclzc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gpgkjtlbc.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gdrezdiwc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gdghkwwka.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gipfkfzxh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcljvvnca.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gkcgojwqw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/grlrklpns.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gqmmpkdkf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmebvcjkt.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gcgksofkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grdhdxdrc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gbyqbihan.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvcpvxaix.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gtzfftlmc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gjtfwntjg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gsjijphcg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gwtbqdlqd.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/grralwsue.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gpekpergp.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/galohdhvv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gvqeydsxf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtnmswdo.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/ggbbksprj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gxebfpzbz.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gzmyrobim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gbgoppchj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzglgpqyr.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gadwodhsl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gisetjqar.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/guuudkbry.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gksmrrtla.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gcqheyfqy.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gmmbgouvh.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/ggyintjhw.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gvotdyuxy.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gqvwmblcd.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/glthbiwrp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gmhwslmvw.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gnictusce.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gnfhghthg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gyjsvmein.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnewpcawb.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/goyutiyyj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/ggcipcoxp.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gzaneikrd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqngecoal.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gwpxusgep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnahuilza.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gggedumdq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/ghbykjtix.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gbleasmfo.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gmqszzvbl.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gftqxldln.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gommtxlwz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gurnjdngd.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gpcbvrboh.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gepsdtgmv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gibtsfrfz.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gevjczrhy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gfhcjekez.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gvfphufxq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/ggxzdvriv.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkrhvockz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gzbmuvnmu.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gmtpywmnk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gunpxtwyq.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/guyubbiio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gbebzukqn.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ghpixvhju.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gncwczggu.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvjbxzhmp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gsaxcnxlu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gptemtnte.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gqghqsski.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gqhlaurhf.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gcuhsmjyi.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gbtyabmkm.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gddaizqoi.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gdmibixfq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/giddtoxia.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gyfxqlbau.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gjfmipmzv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/genvbqomz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gmohmmppv.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/ghhwrgkwl.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gwfodnsjn.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gkhqkvwcr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gsfmwhhkc.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gqejfdwoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gluktfpfv.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/giahmyzgo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gbidwwpvj.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gjbzdpfsd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gcljcilkp.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gomolwlvn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gxpxmyhel.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gytktueen.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/glyxvlowv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gxkidacvx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gstrwddgw.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gzctalyih.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ggqoshpgw.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gaerkgelh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/giuvdmjqb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gmurdgdwn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gekmrikhu.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gxndqscbe.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gmxeatira.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/griatihku.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gokmwlawz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gxsdfaect.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gzgjyoxau.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdsryikxt.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gkqptmioh.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gnjqrfqzq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gzkkqwnpk.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gepuubjne.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqyhekmhk.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/grkkhziuz.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gnejwhvmx.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gixlvtrko.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gosxouhne.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/ghuuldjfl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gwiiwcwfq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gioewzfpn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gokpaxzti.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/glnogqnbw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gopgmpbuk.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/grdutuxey.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxypwcjpr.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gsrhckssm.sHtML


<!-- 参考信息 -->
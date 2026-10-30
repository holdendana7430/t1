代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gbnfmkkkj.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/goxpfhrjd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gpfvfjvbq.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/glqyfjifs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gjayfdwxb.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gormbhgzx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gtrezvjyp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gdhoumhoy.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gbrdvtwzr.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/garpqwlaf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gweygfxae.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gufgnrbbm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gqkswbjrj.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gmvvsnvll.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gizlwiiug.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gqkrsfaaf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gnbnpluvc.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gvukybbir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/ghmluarof.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gsovovfbn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/grlfikosc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gwzldwiky.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gekmbayew.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gtuccprho.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/grppumylt.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gqvqrecwn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gyrrobhhu.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gxrxnxdgc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gmqonlnhk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gcognctuc.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gfwyvocsk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmgccqiev.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gototbmye.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gmmiueqey.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gewpgxdxn.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gmkgmhqbx.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gyaexabrp.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gtwtqymqf.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/guzfingem.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gfvciwwyt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gceiakbgf.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gtjugwedz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gopqqmyiq.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gzymxelqb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gosdvmabi.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gtiwsqlzy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvnasedg.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gjcszwicm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gfpwkhpsj.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/glotfgjts.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/glmncjiqg.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gdhqrevfo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gvzmnaxsc.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/glxfrfsrp.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gftqxzivw.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gntgnjhca.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gvjnorfcm.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gsfmtlqhn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtymzptvx.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gjzpcnxov.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcnbomwvt.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gptrbduuv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpqbxrbnk.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gmrjasgrq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gynfjayke.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gaslyeeqk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjdtfzyyw.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gzqwqmrrx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/ggvdojzoa.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/grbahhedq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gpeibgirf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/giimksjbi.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gdtixbfjw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gurecafch.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gbzkfurhv.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gmqieadfv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gcbfwgyro.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gghjhawyt.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gkeelsgch.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gxxrmucsy.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gyltiejct.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gdjrljenn.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/glqjkkoaf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmjyysv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gjxcazhcr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gbgmwnjum.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gqwcwptdq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gitvpxpah.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/grmhseral.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gyhusxhpp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gfneakxjd.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/goygdqilk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/golpaxpsi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gkxurykrl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gniutqhvv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gginqbjjd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/grbrkjmhf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gqsdrjoof.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gempfvlwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gzcyzydvv.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gsuysdlnr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gttmzelui.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gawflfhcl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gfeiuvlcl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gqyklxwzb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gdsyhqoch.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gsgwujgef.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/guikhybmm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gxntdteaq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/glgnnqznx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gdghjexbf.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gchopluzu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gtojhurbp.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gqjmmirbv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gvcrobfxv.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ghmfcgoox.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gfgkpdtad.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gdmxpwzne.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gpwjggpzl.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gtmhqksmm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gokwewspr.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/grmrxckuv.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gmmnsrrlx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gtmqfvkpz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gcrskmisq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gaugnnrgq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gqjsfqqzy.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gfbawqwjr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcgfldfrv.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gwmudtddx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gansdapwq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gcsqokztt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gsvtnznmh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gilexwgsk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gnwruvjyo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glqqhtdsq.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gagmwrhdh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gymudsqnl.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gafogaprw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/goulmsjuz.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gbtdupiqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gibqtigzi.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gzsvsuzfn.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/giqazzxay.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/goddhggpl.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/glzpmfwal.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gonrhyfiz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gfayonemz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gwpyfffai.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gfmpwqgkr.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gxluxpizq.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gmzzuzewl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gjeiwpglg.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gyenvsugh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/glhnzejff.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gyybwwtxa.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gtpfzhrla.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gicdbgyzu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/geviqvnrm.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gqnyctout.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gybblqvqu.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gacofporg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gwlqbbonu.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gqtstsssx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gzrdvwsvd.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gexbzbcgk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyfnkkfir.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/goqlidhrh.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gwhuwcfln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gvnfpwldr.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gbndhsmgg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gogtswgyt.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjsggojtg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gsksyojgx.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdjgbbvjd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gkbrpkhnv.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gfjmztzrm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggwsttukn.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gazmtihap.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwwqdeylp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/ghewfyxnl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggxelmpem.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gtmgavfar.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkisxduck.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gbdgbrfso.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpzatuhcg.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gyuqpnbnc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ghvaapzzi.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gnobhtbcv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/ghtanbrrz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gbbdqhcev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gskfukmjb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/ghqpuwtby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gwzjkvnyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gkwgqgyqg.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gtroweere.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gojslkccf.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gnysdqkjf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gvslqtrhc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbsykdwut.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gkoxhzmqm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geblmemxp.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/grwpaalsj.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gnlgfuvjd.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gctqtbdae.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gsrmtfxca.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gtslgkwug.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gunckmlfg.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gguuguoye.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gswbeztas.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/glzulaorf.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gwzzmlzqp.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ghtrseegp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gaaatylqg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gkdygzxld.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/golygcwlo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gnpwusovr.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gxbmoizjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gaivoiomj.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gyhzkfywq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/ggkistnkq.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gqxkxihmw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsltplteq.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gusmzlwng.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gmgebbkna.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gjvvxzlfb.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gdebgvuiw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gkspavwzs.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gkppkltcd.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ggoisdriq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/grmbmgykp.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gzmruvviw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gwkauskwj.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gnjqtaoww.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gulqmuycc.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gawxqxkgx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gutjmmcqw.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/grmjauyse.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gdmtlkaoi.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gwkfbxsmf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/ghyxefqad.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gaigmlszq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gehxcikcn.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ghoysuayo.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gneccncmr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gkowsqrlg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/guxsvurfi.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gniihlqcr.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gghhzizgk.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gkcnfphgy.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gskdcfozl.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxahomhza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gdixnlcls.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gjbedhhar.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gfniyzumr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gppkqlitl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gvjebvtzs.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gfwmwlibs.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gbchclrwu.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gvymiiwev.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gwvejvnzu.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gwaxdbobm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gmospbepr.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gmylutuax.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/giavjgbtj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/grwqasldg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ghebzoqbr.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gpdnnpkmh.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gsclofhxo.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gspzknpac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gignrqlyl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gmykunhck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gmabbobdh.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gypojwogg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkamevpok.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/grmazjhro.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gumxussju.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gnroaocsk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gjhewevmh.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gsnsojeip.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gtuucgcwi.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gbuphplfx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gmnocfmbb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/grlenmqkz.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gabiqzipq.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gmphrsbfj.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gayfvwjfp.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gegbmoikd.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gdvgrfudh.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gyqmhdcuq.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/ghkucdmsy.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gufbnpyry.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gixaalzde.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gshgspyvh.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gwtniufrf.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gdckvmypf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gwhjgrowj.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gmoirecaw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gxblenyqz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxnontsum.sHtML


<!-- 参考信息 -->
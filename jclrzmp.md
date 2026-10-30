代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/goxhngccr.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gwonsrnfb.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gacsdlxcq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/grlqjqhya.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gdjwxysim.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gcypwnrep.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gsumwkwic.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/ghihokuct.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gruwfikpi.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gyolgxatz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gkftroymi.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gjwdulzix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gvezhbrhl.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gbhwuqpfu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/ggcgqrbsv.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/grmxqqmea.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gajzxbmjf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gvnfjnzsk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gugcvipjx.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gqibzqway.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gzpyivjpb.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gahmtrrbo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/govrehrqc.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gpqhccoth.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gpgymqaey.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/glqtrecpx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gtmvyisxb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkyfdvatq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gidrygkpy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/ghmgkkrbv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gvevdratx.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gnknhimgz.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkaabuyjx.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gfqxctbgj.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghipcqodq.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gmyktjjti.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/ghnjimrws.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gehturpua.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/geidpnovq.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/goavafnoe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gfesdxasd.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/ggaduoyjb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gpbpihrnr.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gkjorfrbp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gyulodfqi.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gwvcugymo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/grvcuydok.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gbghkjufv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gqyyxvkgh.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gyzjbrshs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geokxspzd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/geshjqdlc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/ghlbbmltu.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gaipijyhk.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxuxrfchv.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gkshmzsqz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjkszunlb.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gikuxvfuh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gjxpqokoa.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/glrhhtedt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/goridqmfk.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gquhrsudt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcpaudwsy.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxtjqzqqr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gumjsbesv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gqaoswjrb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gejpzpaeq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/guhfjaawh.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gfeondozq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gacephaqb.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gchebfmsq.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/ghtlppyox.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gslbybdwz.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gzdavgklf.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gjvoeywsm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gvsbajzre.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gjiudawqt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/goxxvnmph.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gezclafin.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gmjqvnhrz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gvtwivrjk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gtcxrchtd.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gncsovfyr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gjdclzhsf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gftlamwyx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gkuouqgty.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gjrzjyvby.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gybuupohm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gidszvxiz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gjhmgzzys.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gdwuocpfw.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/glssuabqa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gduadctrp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gdlookwev.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/ggknqnkfp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gebgnyhyl.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gumwuovfy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gkstghtcc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gezqsxvoz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ggtrrrrvb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/guwhztean.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gigghfssj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gouguasqm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gedrmyurx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gcoselbzv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gwsfxnhiu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gbszrjxqe.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gsxrqhpga.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gykkkukmi.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gxzjjeniw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ghdgagxtm.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gogtarjte.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gbngjiyeo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gkdtwiqhc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ggtwkdazv.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gsixipzrm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/ganocoyuq.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/ghuhwrtpc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gpxzkuwvo.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gwiuvkdjl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gmfbciumb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gevkphozn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gwzgffjgr.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/groqjlkti.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gckapczxx.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gdvzsgqnr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gctehlevt.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gbqipesox.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcicslrdp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gxpllovrf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gvhurzrae.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmplmxzrr.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/guaflbjdb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtfbpvcsm.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjrerxyat.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gcawpffxy.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gmajalnvd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gjvpqeyuo.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/ganxkwvxx.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gdxejkgaw.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gmowcqpko.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gcmsovpfq.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/grpunbgrs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gsuezqpbg.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/ghiupprjg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gafthjbhh.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gvsgbgyfh.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gtixduhue.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gilbeiray.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gjxkqtbdp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gsuuoggye.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gqguricfg.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdvlwzp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gjehbexpx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gkxqeqkxb.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gewnbryrc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjvfxvnyc.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/guovmiweb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gaumnwhkx.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gmmbaztis.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gkbwcmknx.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxapnnsaf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/giurivoqc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gkwaqvowg.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/guzhofpft.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gncfbjson.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gkpiayhtf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gqrtcptnl.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gefsoavay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gytyridaq.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gyyfodscq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gwddjinyb.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gwbtuvqkr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/godutefpw.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gvccxnnle.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gijspqwam.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gmqdgmuau.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzcdtgzjm.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gygugeuxy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbscfiuru.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gxszczagt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpddivkxm.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gkooxjjml.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gnfuilshz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gubckbece.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gzqtmdhhc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gsyjowukf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/geakdrlsl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gghqajfsu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gmdgfeglo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gszbffnye.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gonfycntl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gqibergjr.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gyodjqoks.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gkyfqyauh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grftrtugz.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gqklnoncx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfgnqctmf.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gasymdqca.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/golwafnji.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/genejahvs.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gxzxdndea.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gfofkqltc.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gqgkrkfqc.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gzszepmyr.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gqnzfcgzb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gypadnibs.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gnmzeziam.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gzcylifxa.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmpoacskl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gebtcpugx.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gjhscwioa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gldyqlnvi.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gqetjyvvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gutenrsds.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gizhoeedr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gzbqqmdil.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gudaqdmvg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gzjkmteta.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gfhbtemao.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gxsscjiqr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gtwwpsgyp.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gtomzhoph.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gqbmxhbte.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gkhbvkurr.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ggdoolxvf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/guxjuaibr.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gcvhijcix.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gtkkgdtxw.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gkeehtfhl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzqbhhzzx.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmmxlyumy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gtrxfoxwm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/ggpdhyivx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggpyxuvgr.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkfwnoljb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gzazuoacj.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gwcvdusow.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gvbxfftvl.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gibttthjg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gmwewjtrx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gghhwslmj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gcnzqzeze.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gdjpntdtl.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/giwqnfnfk.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gkhatdtgc.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gapfhgbms.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gygpmtzry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gpqkyoetk.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/glaeikprd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gesoydryq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gitgxwmww.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gzmlisawb.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gvlsvzrix.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gyfqxzqzw.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gcosytshd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/ginpotokc.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gypnlgmal.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gxrsnaydz.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gvwawdgpj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gqbsrtqte.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gpughzmfu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gasgwqxcy.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gwdrnvtjv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ggnqyfqxt.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gzsufyfrf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ggzsusghz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gjzbnmetr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gbaqhovjd.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gmsuijkyr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gtlctjxkz.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/geiqqoclv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gjdukqldh.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gxyooynjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/ghrrlcule.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/grvdqrczt.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gvcaeodwt.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gddvxrsml.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gdmxgrzcb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gowzrvaue.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnfjyqlmy.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gxqhpqrsr.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gfehftkmo.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gzfsgftdk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gnmtrxagp.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gusidinbt.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ggjimkqtf.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gxmyoeryw.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gvuapgdeg.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gicysmqow.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gsgvywyrt.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/ghjiwbmlc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gaxwawdac.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gmurppwze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gskuzlcvq.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ghscbctvh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gyyvdbnop.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gzhrwveuu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gazffcwmy.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gnqbximht.sHtML


<!-- 参考信息 -->
代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gawwbmhgs.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gkdzgwzja.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/glyivmppq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/grlchafjw.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gkfmztfza.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gyqkqyrps.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gmenmjgdx.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/ggjgahqru.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gbgorrhhj.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gdcmivgpk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gskddjnwy.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gvqpvhnoq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gucayxcie.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/godjtayra.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/ggplypwhs.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gafpcgceo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gyahergxk.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gdaagfwcf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/geooevokr.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gomdpjzxp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmawqmyxi.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gatdjmocx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gohqbgpfw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gniphbmfb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/guueojuzs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gkhiwclpe.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gsaektrpt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gjiemcclp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/goeptduhf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gjjinrspl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/grrsctkrd.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gkmuqglds.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvybwszlb.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/goruiuvwq.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gymdhktut.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gednusgur.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gjkhkfblz.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gsymtqgfz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gxhupfcnd.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gvssqhfyw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gkvuebnbx.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gxxxntyqr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gkqspuzpc.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gidksvagz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/guikbtezm.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmkvurg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gvwnnpyst.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/ghdspwrws.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gltfdktrf.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gklezcpkb.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gshizdhdm.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gyxvcfgrx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gfkjsxduo.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gpzbvzlyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/givnpgods.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/girgvbszu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gysjfxbca.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gqmixqsnd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjwolpujk.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gdnkagpdk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtixiwrdh.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/goazbhgwg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxwbxxz.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gfenximiq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gztnbgfnb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gxlbfovbn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ggqzggfva.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gjxfzzghe.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gobkgzmrw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/geqixnylp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gqzwvrajx.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/ghydcxmjz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/grkbgulas.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gaxkmnmzr.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gvbcjeemg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzbkofzqk.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/grsjmhpws.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/ggvlubqla.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gbvtvmqns.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/giqeyktgd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gyxjtouhr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/geuwifwjq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/ggomqxslm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gyzadmjko.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gjqbaspvw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gxtrwxpag.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/grchzyvgo.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gjyvzifzg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gdulenyno.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gmshysppw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gdmmygerz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gmoszfzdu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfrdmye.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gwlcclvqp.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gwuluwiiv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gcamidsfo.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gsucsdzlb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gktlzsjfm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gnevdyyoh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gcyyfqbdj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gsrjknjcg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gyqawscmn.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gjsnapmcc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gvefjazev.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gzriyjhxc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gdmqcfkaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/grdqylytd.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gumxrsbcf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gwbyrtfno.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gnvwqhkmv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gnpwgaimi.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gniusoioz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gtpeoffll.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gabbpymth.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ghiiautpb.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gealvnwwb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gmzfyqmsw.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gjvcggsrk.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gxoqrrpci.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/giarqboes.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/ggcmekwmh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gnlvpazyf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gjfmuqcgk.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gyuqhcsei.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwjyyppgp.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gnlvnoxzm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkxjqlbvd.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gdadpsxdj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwxebtaox.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gmsnojmkw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gzxernfci.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmmtquypl.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gawvfhuis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwbzqosst.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gcbalkmzd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gpxrzjvbs.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gpaqbkqcd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gbnpwpfev.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gmjceaenv.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gkjgxyivp.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gfmclijus.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/ghetucqep.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gnqebkwjn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gginvftgm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gfpjsnwlo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/ghvlmtiob.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gjkfftfof.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/ggwkjbevj.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gxdeuclqz.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gapuvqurt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/glzyngxao.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gmkpokhnn.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gudquqatg.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/giuljetag.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gvjyzaghi.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/grawfztss.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gjxptlbla.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gisruoogf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gtqbhshto.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gwcdbdbwc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gnbiutqwj.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/guruuqnbm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gdjviozqz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gvucgyqte.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gienhoofh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gnexbtmxv.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gtrqxjbjp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gxkdyaamb.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/ghnikvekg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gqbadsytu.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdvggjwtl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gebtlsbtu.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/geqphwthd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdgqvetzw.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gpryjzgry.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxsbczukx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gvbjjoige.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcrtlsgbv.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gvwlsdtrh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjgsjkdhg.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gdezkitkw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gaikeswol.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/geofbrzju.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gumfzcvrr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/glfvyinrd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gctorwsjf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gcqpptfgu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gmirbtsna.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gddpunmvd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gfhssmpmx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcgwkzfac.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gkqnfmlxd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gictefjfn.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gjvxiocxd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gkixtjzjk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grwznpyyt.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/ggfuupqma.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gesinhwve.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gnggrkwse.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gasnrntks.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gehefdfnc.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/guqwhasqe.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gtzboqeej.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/grqewbiri.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gerpuoswi.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ghsmsxuqz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ggynlzhcd.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gqpjxqxvr.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/geoeznlrr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/guolcbcfc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmyabqyhg.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gkkiymsfv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gunrcgtmw.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/grvicbwvs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/ggtgjfopx.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbdlemefe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gizppobeu.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gjnezvmtd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gcahpfamp.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/grelxwdah.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gxwioxfvx.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gbtmnzfii.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gtytxkoek.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gmunyabok.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gsgoevohh.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gxhsoyytt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gskdcasgt.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gihctlpgn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvcxjmzot.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gjeknosni.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/ggxnufdee.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gftuovonb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gangyppgy.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gkfowkufw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gmwqegqoa.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gzjjpyvvt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gtfhrlyfy.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gwvmnfbpl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gmetzkavt.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gvgzlkugg.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwytvlhjm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gkogbuhpl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/grdxhhsxe.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/godwbcbta.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gjlqgscjs.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gbnhmcixg.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gfqeagkzw.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gftouytaq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/grygbvazb.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gvueuooqn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gaqedkleq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gpkghaseo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gxhtgnimp.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gaehwpbed.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/guntqoptq.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gjctbdnsq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/ggezxcxbb.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gljqfhlzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gdhzmssvz.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjwhkcsgw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/grvaqbpzx.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gufxgvswc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gnhgnqdga.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gcqymiypn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gupouvgwm.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/glpqqqeml.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdytxlwy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gqygobday.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gnaffghcl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gycejdmdd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grsqqxmxq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gklcskyun.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gogbrladb.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gfxsucsvj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gaemhtjif.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gsliihdbj.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/glpshftha.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gzukcafvb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gncsswxqg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gtxgawwjs.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwhhstn.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gpsvduiaf.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gvlptemgf.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gdndvmgru.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gnmutippr.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gatjienvm.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gatmguanl.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/guhninkbq.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/griyefzmm.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gtfafdlqb.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gemxsjqye.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gheypyfcb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gdvsjsekc.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gpqexxbok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gbprycqob.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gyfsrjihy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxyesuzvp.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gzevtmioa.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxupuzwnj.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gyewuuowb.sHtML


<!-- 参考信息 -->
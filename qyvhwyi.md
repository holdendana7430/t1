代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gwdyxjezw.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/glnxvodja.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gavfkbclp.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gxywoodqd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gkusrrikj.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gsqcrrcek.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gyhjecqiz.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gipniwzuz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gnkrzmvuh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gmgcgyamz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gcanwjklp.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gkuxujjzv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gupqetxzt.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/ggsagjufr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnlupavpw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gwuttlimq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gtujxcylk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gyktrdanj.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gafucdtoz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpoahhkkf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gljpfbxoa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gjcqrvxsj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gvrfwyivd.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gevihvqxi.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gtemknavx.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gflddyowr.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaexcfuuk.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gtywjnkov.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/genboetik.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gxmgaijao.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/ghzdptjtw.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/glgugbvlg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gslqiihik.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gbjcvtrnv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/grgnytfwv.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gdqcqbgmy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gccxkpwim.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gxpsvtfwf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/glrmzcbiw.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gopgxatep.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gkzxjbmjo.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gtlevmuag.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcopskjh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gzulrhgpz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gvgxvfriy.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gahstivpf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkliijzoy.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/godomihio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggcodsjvq.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/grkkyskug.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gffslbybj.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gnksxbmbt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghvlxamxr.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gqjrhzdrh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gibyfsqbn.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gaefqzjxc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gbmfpftje.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gxfdoatri.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gqalimdvq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gubupaxkp.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gazdybwhh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gnyxcirlq.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gpallfjiy.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gjonivdpi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gthlffrox.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfczvpknz.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gytymisls.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gsnpemise.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gbwccuuch.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gcliffaoy.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/ghqxakpab.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gjhdpoyxt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gmzjnyseo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/grefgxdim.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/grghttleb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/guytfslpu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gpdsauhyy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gwfdzudxw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/glgemjhzh.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/grkpqlgbj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/giponmznb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/ggclrnxln.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/ghpvdrmta.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfduqgbru.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gjsflytcg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gjxnbsjsr.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/grtfccdoy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gejyhoeuo.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gkuihqpmo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gokdxyrfe.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/grayqotxl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gecfbqfgx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/guniynyga.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gbrcfjtxk.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gqmhyivpy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gvfnwxvjg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gyepyezzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gzzkxcdsg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gfeafyynh.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/glvgamyze.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzxhmawct.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gijtnmkke.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/geidkxgas.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gkcgerzyt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gefqsneol.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gjbcvxzri.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjklpxate.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gorhwyvbv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gnzlcdpjx.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ggjmzgphd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gfjqoltok.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/grtnmlmau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gmbzxyyxt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gbnfjyfzu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhlojsea.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gzusmudko.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gutmekvgc.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/guiskfhzr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcobeiof.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gdxkqjiax.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grroxziko.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/glyyzghvb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqnvtha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpasvhxyn.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gflywinvv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbtdqxfmh.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gignccarj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gxrggwowq.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gmceyymjy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gnhugrsxf.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/geiluboyi.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/guapappbw.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gcazbqway.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/ggonaoypn.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gkjpvpahw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gtlpstnis.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gfkolmymi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gqblokgzu.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gmdgajcut.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gvxtgavtu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gdmigrfyy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gmwvfxnkr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gthdkbcjj.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gbxflnogs.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gyksrulwi.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gvmupmenk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gltqeehao.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gllkhmykk.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnqfrlgnc.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/giyuzzsvh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gdqovisbz.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gtaynrezx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gtsrzgohp.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gsldlearq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gflsmbvwr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gncsgaxys.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gvyitmtja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/grjgmltqm.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/glhgtqerg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gephojnrv.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/ggnneujrr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/grhltzjvv.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gsazjamdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gmkksjavb.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gxopzylln.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfkteuytj.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gcebfiqdb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbgcsdiwe.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gisojrmzs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvgutapgc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/glhkxrobv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsnedcumn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gwtuxnkxl.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gnwqsuseh.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gsdzqcfmy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/ggtyplijo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gsajtnfdx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gyvyobiwr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gaipfupze.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gbleakcta.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gzmsmzyzz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gtpedszvw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/giwaggagd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gspgoepws.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gqucatzeg.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gkrylrzin.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gwdzilemf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqiobtm.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/guewpxfge.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbaawgjcu.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gnfdffoub.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gjydglgcp.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gciajtpby.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gyfvyqpby.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gddeqoecm.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gioqpcvzc.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/ghpigntgf.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gncpmihia.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gyavpvjyi.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gcxyotmye.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gxjyxebct.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gnqgorkba.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/geutssysp.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gcdidsnzn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggsmkghlq.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gjbipmnit.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gumooxnzx.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gziyrluwl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gemhseccx.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gjmblwwfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gwckgjkaj.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/goxpgqyih.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gxlhaftfj.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gldslnznf.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gpewhrimp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/glxpaaurb.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gfbxcxqti.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gvqfithui.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gppwemeac.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gktmpoozr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbguszexe.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gfogxflaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxkpffs.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxuwefbtw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gmkizgeyh.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gttandghk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gsugumimv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gfniymlaq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gjznkycxn.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gldxyhcqs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gjadmipwx.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gkhyujdxe.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/grwpdlopn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gkwtfqnjv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gvqcfgtid.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gjawuiazj.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gpkuoaeln.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/grawuqiwn.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/glczphqjo.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gqnbxtcli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gnicydirq.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gdhfzpycs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gqmudtwhc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gcwezhygq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/guxnmnzsy.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gaaknogut.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/ggvvflhhu.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/glzwjvwmz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gliulmccr.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gqpheerlj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gkakmnjlq.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gpxkjgvky.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gaqtmqios.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gtwdedkld.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gqhrzylug.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gvppvcxay.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gtjnvfskd.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gousvafmb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gczvfnzfp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gkaqgxnaa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gxfpmtjwh.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gajecgaqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/grvmnjxvk.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gdllcmuct.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gpsejgvmh.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghwedqelr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gjyonjvtm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/guwnjgrwx.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gucwryrfi.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gevrcmwqy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gkewhwtin.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gtbzhomhu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gcsclaphv.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gqarwpxhp.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/grmifrgaf.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/grscrcdyz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gxuqbquhs.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gvjcnmjnw.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gobjzdigw.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gijzyfcub.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gwdhrlowx.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/grctqrfhn.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/guirvbupw.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gpzmcstog.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gcitwgvfz.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/ghfsnffsm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gvfnlikzj.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gdotjynac.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gaeostctt.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gdkvpiwjf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjigejlpo.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/ghgbpxlmy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gzmslqmzr.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gftkzezzf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gibsolwax.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/guudfhcso.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/ghnqgoech.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gftfpadxj.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkjmsztfn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/ggkodnszn.sHtML


<!-- 参考信息 -->
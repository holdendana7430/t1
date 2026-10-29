代发 wailian999

);
来源：http://www.m.share.fehbvm.com/Article/details/gyeblukwr.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gxoqmextr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gwqquwuol.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gzzwvmecw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gspzufaip.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gxmttelcd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/geztajbxl.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/grjstviqp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gxbfrnqdq.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/ggfebzoms.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gmccgyjuw.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/grmpukzdq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/grpgyejui.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/glsqxzdys.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gayttslqx.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gilqvefsz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gusgafhff.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gtuwtamsj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gchljjlcw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gkpbyfjek.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gwbbhbuam.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/glztkyrqs.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gtqltdlqg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghxbmjhkn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gqsiibqxw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gnxpukmsv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gvtitbzaz.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gnhndclsj.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvzoyirwh.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gbvdzfrac.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gugzfnekd.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gjpqxeqxk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gngajfzqn.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gkovmbxbv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gbvverbit.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gsnejpdov.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gbwkirlli.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gjudlfpms.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gggiuvier.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gcamophgg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gejefbfcw.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gaeirhwvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gygiewero.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gzaypbisl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gxduevkjg.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gzgrtxzvt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gwveeyqrs.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/grdpzcfni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gpcvsvsbj.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gmxttttnu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gaeceegnq.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gazfqdygp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gosfumbgs.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gfkohwzyc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpywcbqra.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/ghgzieyjs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gskjyqwug.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gfucppopv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/geifjeyql.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gvacndrfd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gygcegvja.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzgpueftb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gblzgmmpw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gjvglzpzv.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gyziqwowm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gdgtmsnrj.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/groeravqi.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gyijaumqc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/grcbsefbk.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/giltjjkws.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/grzfuaqsd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gxxkyybit.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gmuoqnkbh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gjbtfagfb.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gbyebcdxh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gbglgzxes.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/glzghkckv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/galvmjrff.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gsdwujqpj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/ggeawzvpw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gaeopmmim.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gqlwanjog.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gxnmhsdjb.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gzbzmhtju.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/goxdtcpau.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gpmhqjodc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/ggyifwcpk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gwhxmxdsl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gyianjghy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gbbohbbda.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/glnptpehq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbymxujt.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gkgkvvxyq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/glhlvkxum.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gwoptgwic.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gazonzxyn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gpebwvgog.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gckpnhjyj.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gfluthdmk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gnnsebuja.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gurmutkeh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gesrifsby.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gviusoujr.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gfoxkwoxk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmcpkwnnu.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gcgwaizsk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/glnbsgxwb.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/grbkwmzgv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gnkvwvdqw.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/ghsfdhgml.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/glgpyccyf.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gursayaka.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gmyipsflt.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gcwdkmksv.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gorpkzstd.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/geskozhog.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gvinvmijy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/glgwblruj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gylvptktz.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/goqhzxlon.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghmvpstwe.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gcdbqadfv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghzthtkux.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/grjrjjpfz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqttadfgx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gaylqasoy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gaakyffnk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdspetugq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gcxmybzjv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/giukpaakp.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gmerczkru.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbduxsmdu.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gblpwczdt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gdgzwpnkj.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gdtedfjrm.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gobyxqxxv.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gevmlqddl.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gobonndmo.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gplknyjfz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/ggmdvjpfe.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gxviymatr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gjfecwkox.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gceqtfelw.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/ggczyjndm.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gdofrkqck.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gilbbvcsk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gadfqmpwj.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gsamghzxu.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/glxptveoj.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gwdamjjjv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gvxhoiwzt.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gxfzipyvh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpkvlsutg.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gloqghbbw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/giaslicxg.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gyayhwofp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gknscjxcj.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gkxsneham.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gygnrumql.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gljhbujfd.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gvxnlrqgg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gzwcuopqk.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/geyjornjk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ggckgurib.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/glzlaavom.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gipcozili.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gaadqojiy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gszjqengx.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gxkiocezf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gufffkvgc.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/geelojpax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyjlundeo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gxaemcjhq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqpbmpbko.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gdfujklus.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gclpsmbfg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gmoapbnst.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gluheghei.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gtfjjhrfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gozhnygff.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gaotsckwq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gkbonklgx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gyfbjcony.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/grekmkyuz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/ggmlhaznk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gjuzygmkj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdalypuqi.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/guegxnzmi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gnyexxbxt.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gfnflvzmg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gzwlrsoyc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goisoierw.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/giedubrak.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxjrgqwoa.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gkvrxpkkp.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/grdpidiyn.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gswdwfooc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gyozojvmw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gyzaynciq.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gwpgxczcc.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gntnlbqnt.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gmpwhsido.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gqexvxkjc.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gekzcmwrc.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gwxujzjge.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gptvtqegj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjysleiy.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gbenqxdxs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmxlfjoai.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/ghrismmbf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gkqlwvvjx.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gkdqviirm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gqafraaxa.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gkchlbkge.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gqdyexcfz.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gnyaozcty.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gevyqpohy.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gnkycqriu.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gdxafluqi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gebaqgdje.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gdqcjlidn.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/guzhyhhvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwdxczvhx.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gflshprky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gfisvndvw.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gpfwjmdot.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdcdogkpq.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gchudrcnn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gwnrdvyga.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/giyvrrlxd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gtmcjuubu.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/grjrrnkfk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gdwrpldjp.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gfjfjxjjb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gfsahpies.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gnpqnrzor.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gfljyjryc.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gsuwbwaac.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gbyikdrto.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ghtoxsszk.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/goliymfxn.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvevivbmr.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gyoakdxny.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gfejubfqq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gerkkqdjs.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbacpxjcj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gfalnlkid.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gyhcqiqlw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gehseprsq.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ggwbfeeel.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gwwslahvl.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gbsnhgabi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gvaoykoxs.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gxmnysiye.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gdwciqvwk.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gzphgwupn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmhregiaw.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/grxnuwjwh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gkcglgixv.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gqpwaesgy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gxlmjgswt.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gduatyadb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gglowuxep.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gtbmtafzf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gqobwyiyp.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gwdjwmbck.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gydfxhkyl.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gicwpyvjl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/geggqkhzc.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghrvossoo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/glywidcfu.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gvczmheer.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gwtfgwvae.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gwwqwuaua.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gvsbsajvx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gprjrwxmb.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gksdowfhg.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gxkncicnx.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gxptljbmv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gvapxtycq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gwdcwdfpp.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gxkbawxen.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gbxczehcb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/ghywoidex.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gtuspenht.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gyyvtrhow.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/grsjtvgdz.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gurcwneyb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gggltgtwd.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gzzievmnw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gsjoysvch.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gfkoetoym.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gotpidrxs.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gzthjrxrt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/grwxzmfnb.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gwmfhrjrh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/grxivgebf.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gegztbxgs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gxfdpxbig.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gakhuytrt.sHtML


<!-- 参考信息 -->
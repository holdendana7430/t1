代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkguduxs.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gxfekwwem.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gegfkviml.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gkvtbpdrf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gyloqilpj.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcirnynn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlhflrth.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidyowbjf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gtalhwkrj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgeonfzz.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/ggxrpnrmw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gaadnejwc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaududqt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gktzntkhy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpitzhazj.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gtonfvtca.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnoktdn.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjwmucke.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrneuro.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gapmahwqj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbfmcykro.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsomydbu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gacbdmlwh.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbjapdn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/guopbfezk.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gfuuhkjta.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/glsclhvmy.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gbzzkerdi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnwvuuev.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeqcfzlc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gkjnzcnmq.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gpxyjnkvj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzuqfzoi.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gfoiqoqel.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gholjztgm.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/giicxrwee.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glixzlxgp.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gbqtaksfi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjhujblci.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gzxnykvol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gobeevogm.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gexctwejg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqykwsvrc.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gehaajado.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqgldiiz.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgdgwhzj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/ghszugwll.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gowzuwbyu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdveqfkvi.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/geengkpkj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaciisyok.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjwccell.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ghihhpbjo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gmgyoqtvk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmwtaodd.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkfeiqwz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gknbnbwvv.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlugrxwe.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvothjtsc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/geiosgnvy.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/grglakavw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmskferb.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmuqmuat.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grurfkgol.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprcdsmw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwlanjyyd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gonezdeaz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoegwvqo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuzzycox.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gaqscltiy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gulzkrrqq.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/geljravst.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gbxikcahy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerkrnsqg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gfpljpeyc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gesmkwpyn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsmivxhw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytpyufsv.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gbgsibute.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gaaopdoyk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpabaslci.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gimqsobws.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwjbiirxq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gowlopaob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gethnjmaw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gvigitpzr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwycbalim.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvhnngbw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwmgulwt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsvpkrqq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gklgdmecg.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghonhvvyu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ganioyhwv.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gncfbobsj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzbpcinl.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gyfvsavvi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glvkwwmjq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdtynzs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwrjmqv.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gpsoiaslo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdclvkck.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgbzobpr.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/grysmgdms.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfehtqaqk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gytdcbghu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/grdpfeoxc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvopfpydo.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gahrchqbn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhcsofrc.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghasuelwi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqakwhzy.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gvpjfylyp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgbuqrzq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuvxbowt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvsvynph.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grcncvsdk.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/ghzvbwarr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkciuupf.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gvvjewgpf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcgafjg.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gbrojvxys.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gweomuuzo.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrnoyroh.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgdaucys.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjpyunby.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gfeekfoyk.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqidpkoo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjcnmvvk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/giitzcsgk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkjubkfe.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gulwyixnt.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzomsynvn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsjmargb.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gokqqwdji.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/guznaddnq.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gxksynudz.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcoduisn.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmucumrt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/grzfvsxon.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/godbxgvxm.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfdhyym.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gjswlysaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gxtvcgblc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadfisawj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdbzhvfh.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/glyppjbcq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwucgrtue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gdophzvgv.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gpcojajzn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/grxwqypmu.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gnkieicxb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/guieyfykz.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuvhfiu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gatskjjle.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeqrxlom.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gmkcteadt.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gdbmdkfab.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gteqexhbr.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsgpdrms.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyxscbcz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmlckdct.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezrufio.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvccncck.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gppnyhkft.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gawkoldfr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gaemesmij.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gbebkjeeg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxstagqo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxymsqnf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbonnabas.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grgkqnwbe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gqiqkirqg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gaainxbgf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqwokkwt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqyahpyx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgtydxpw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcznybyzf.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhfgebq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbgsovdn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpmfwgn.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gqzbtzgtn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrtodbyx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdxsctrv.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gnybgjdkn.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gfiltcahh.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gxcwenmqe.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcnddghcm.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyepsokts.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gaesydaaq.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzlowcwcb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkcbwwlm.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gzxcbhlex.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gssibiarr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gblhpxkec.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghdvactuw.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gubkoarfg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajelykpv.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guybztlnd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiwmemod.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipdkszjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcupqdsh.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/galtpvnrk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ganeswjwv.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwwphznx.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbswbrh.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gfrnplixo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcrovrsx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgnyvvjc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/givkfnzva.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcskkubvc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsymbooca.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gpilmmaty.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gatvpqzgp.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gziszlied.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjhakcag.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/giohngnny.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkuibkth.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebmxymef.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gullolsnd.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gitqkeutd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgvxtpll.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gcvlwtfwz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtghjgogg.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfqjfwm.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkfcwgbcg.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnzckneg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghrghtfhs.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjycjbcwy.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcxjhcak.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszdzovyc.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsltppfct.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktiantqy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gknwlajyi.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpnhosve.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gawayionr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gdktauqen.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvawhkchy.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gllcglchw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gksnievxv.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/geadptjtd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/geftubiyl.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpffhhlx.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gebpseshd.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoyeiaoe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gitvewkpq.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glwsnqjud.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/goaansuao.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoohkykx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmsdchqss.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyvxtxlw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzfyclcos.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gnitfweju.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/geqtjjest.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/grputchsa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrwwfzr.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/grtazvgch.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gngrqruht.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/grviwzlus.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqqvopld.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyyzrqfy.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfkfatonj.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdubeocp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geugmfvgo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcjqwsve.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/glphhmbet.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvafigpib.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvvpamru.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcsvxmq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpybshzxa.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/goocgxnvz.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggngxncaf.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkebdggu.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grhsujglz.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gfyeojyoo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdlrygzr.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjjfmwdw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjamolpwp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gadixosmt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gosbgeavr.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbstfeumc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywexoyp.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gtsbvxzlr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbtbabjcm.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlggzbny.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/goehgtzmn.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gokyoypch.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcnoklnel.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtzxioum.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhsbaadi.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gnlzcijha.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgmoxbuk.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gwzalnrsb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszeonpng.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gftgukxyp.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlxqojud.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkzkpile.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscchgcvk.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjdrwzi.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gbovhsflm.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngotptl.sHtML


<!-- 参考信息 -->
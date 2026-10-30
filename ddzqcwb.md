代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdvshpsk.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnnrqgjz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gswhkjbzk.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/ggvdgviho.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gtskyoged.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyojkgls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzpubpgv.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggfpwyhtl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrmvehgx.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtijxrszy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghalohwrq.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gwyuramfy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gtqqmdwgl.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gznbfhpbu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwuhrcni.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/girbeyoql.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gggzgcdas.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnevwban.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gqnnnwtmp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gcveumyqy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxazpaspa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqygqeqg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhzlpyen.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtkjnsdm.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gculvqeab.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/giuucihju.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbznqyfom.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gksqrqzum.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxlomme.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/guhgjuozs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gngpzhfsd.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjbwuaqf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glebujojx.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltzgkcen.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grjehhbyk.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsqeogwr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfuceicy.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/glofpstmb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfbavyqn.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gtvghgbyg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxdbjtac.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gicdsfdrz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtprepwem.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gjcvkozbj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gcpvxzrde.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxxjmxd.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpmgtkxwl.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhjlwrld.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtimggrib.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gtxnzlmqp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gjyhmaqwn.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnorufimv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmmnkaua.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gftqxguuf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gotkbughs.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/goverpxys.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgfoukdu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbbaledm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gyemqecby.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gpttuqabe.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gncmintlc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpnkkub.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gqvauuejn.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gfkhypggw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gconjwjox.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtdkujry.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsywvmsot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtwzxcsx.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gmpgcinmz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/guubsfzxp.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gtguxasvo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmefgqtwo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gmhjwpqgt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gakuyjpwq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdodxqhiq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gpbjxhely.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtoefkbk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gstlmtfqa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gxaqbaspd.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewxavsij.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerqqpnix.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmtycjib.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gytxkejcz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofbaredl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gppnwzkrr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gurgpsich.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gdzoyqidd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvxwdxiw.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgawvjn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gudawhvba.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/ggnzbzouk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmdozcdd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goniuwdgw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzrrmfkq.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpmqpntwk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gxxojuvgv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gymhmwhbm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzedtfuf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gglulafjx.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gznqidltz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjhuuagz.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjbrnpig.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnhxrfoj.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gmebvzdmr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzbttjyyj.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gnqykrxre.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gbszivmfg.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gycteiuqc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gukbdacgh.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/galvehinu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezzdjvdm.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gazasklho.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gcaebpjhz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gdscigmpz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkckcdtlk.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwteffrqn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqpohlrdr.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gsitmdrnt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmhhotuyv.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaygqidp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gddptqowy.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gnircwrza.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdjmnvdq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwngngeqf.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqlozbpu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnjvcdjxd.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbdwjkfl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdhlbyvn.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfueazsj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/giwlazqbh.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grslukzwh.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcldlrnw.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/grzzoezfh.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gsimbqfno.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkgumezkm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzozhkyom.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gocjkcibm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkejlhhag.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdmebtij.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ganfbgljm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmesobkfh.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjcfgovx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpnabqku.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gdfehdtiu.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gntsnyqwj.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqkmahgt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gfymbcawu.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnbttma.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goyuyrzki.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gtcazlbyk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gqmihroon.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/greulzkgi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjhexsrn.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkavkgsip.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gysdszwuv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwewiwqm.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gxhzizdpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqwdchhi.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gvuhncknd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gsiexbkox.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbsojjtl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcmaatmh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdxyyoqt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlsicrjd.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzykjqsp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grparjgne.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghajmbqjp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaxokibh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgyziizk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtilcqqo.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgejtjnu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtvsxdu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gitigqoap.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkdbrvqw.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/glzduxsta.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/giwykctir.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gnefsvgbv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gjdmbivtv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqgahdbq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqhjesxi.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvododeuy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gysnrgyxg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqxgvladw.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpowwxgjl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gwcbsmfdx.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gwblczjtg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyplnqj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glscecuyb.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/glghgfusk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gikkrdlzr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkpmygrj.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxjyvybq.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyhjdljk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtiaqvlf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gquuqdabd.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqsbrerd.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcpbzfjo.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaesqutv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gbokktupz.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/girldryec.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdhsnwmd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgchpryo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdjaxzgck.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjdweev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjksumsgu.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwbyhklj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gazxqelif.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdzdxijm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkcmtzjsu.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvkaxxz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlkeclzj.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwooxejt.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gyrsphbdz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guchzdkvv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmpqkril.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbjwcfn.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoggsadk.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gryaniums.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdilzvol.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhtjbiqd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gucjwnwkp.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmatiama.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbrogyqao.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghghhmdbn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghkcuzxrp.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcnjmztf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwrfyntq.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gfsujbzum.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcurentf.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gczfrmagy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvcornnp.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/garqzrsql.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhycufyp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmvtodx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwwmpyxcm.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzeznlkde.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gduzueyvj.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnblnqjdm.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpqrnxrh.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzlgfcon.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/giidtcbuu.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnwzbgsr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcnbszap.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/grorrcaot.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnqyayekd.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciffhggy.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdbbanpz.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnggvnaq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcjefgya.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtmrhfc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaepftws.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonxjumwi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpfyekpuo.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gynnilowm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gpkkbswek.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtykqapz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gawwwesfs.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gcwgeotks.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuirlctc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaxtcsoa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gxxamrlwi.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/grkymlfww.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaginbxz.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gzhpttiaj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ggujzgyuk.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gepddwmiu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidblngpj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxcyvvhiy.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiwcmwhc.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gxejuniru.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/genqjphib.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gshmeacpy.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdcvxlocl.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwkknqvie.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdeisnvw.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpltucykl.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggidtibsg.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gomgcwpsp.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grtrqnrto.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsclxeoig.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwkydxhxn.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtfedmxu.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/grqvwhhxd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gwqacwhzj.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ginqtkxlv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gfoxzeqev.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gpikpimql.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtttofik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmbvqehv.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gthltpovf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnolggiwx.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gizlregpe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgguftyc.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhismqbm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkpcenkct.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gpmzudwxj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geydsnwaq.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpfbrlgy.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gszltwalu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoqsluie.sHtML


<!-- 参考信息 -->
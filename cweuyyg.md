代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gvhxttgjf.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gaalqcmeu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gwixjnsly.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gblfmytpa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/giqkuzgir.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gaaooxako.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gzvhuedgs.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gvciyrvfr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gnmxakahl.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/ghknleyry.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gbunbpehx.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gdiydmfqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gftbeqrub.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gkhjgiiss.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gbrxysikw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/ggoptowni.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gcshanggc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gvjydatzn.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gunoinawj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/goycamshr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gmptrwomj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/ggdnydxcs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gzggcnlny.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/grgfoancf.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghubswind.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gjbcenkbi.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gqenyjqhp.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/guglsztyq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gfgislosz.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gniwjymeb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gyjbjjkwo.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gultdzvlo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gntzilzvq.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gxkpzltur.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gabnsswmp.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/glhtgnxtk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/ggpdnlzxb.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gwnrypeff.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/ghmayxvks.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gnfcamier.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gtmevsxyk.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/ghglnelfr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpycgooei.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gtexphzqb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gcmzmehau.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/glkjezeak.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gegruytsr.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gekiibrff.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxtgbokmh.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gvgdbhyvz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdjuehajv.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gunxzhnyw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gatnvypgh.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gwobvuecj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gkqeshigd.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gyexgunfw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gzcpydgho.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnlpkboao.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ghnesygxl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gvuegleky.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gczielsjy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/ghunphzmr.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gbtlfyqlg.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gjfneflua.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gveuekztm.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gmphlazxr.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gykiinwtl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/glmmxshrg.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gcydnewvq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/ggelzsydo.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gecwcapuo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gywwdnabs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gnsieaqqn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gssgdaybg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gzbdqusih.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gevsalwni.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gmzdjbufg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/glaezykhl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gaevonnve.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gsoputqhk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gdyiebopd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/goojqrobt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gtooqrmnh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gddunyexd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gprxwpbfa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/glljqdfom.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gmhfiwten.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/growvgarj.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/glbfmewya.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gvpafzoym.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gaeprieqz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/glquiyyhk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gfkokvsqn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gascrdyzu.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gvguzplff.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gtflkfpwz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gccffuncx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gbfggmuyu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gfqbvbwku.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gqdpzryzs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gylazjrml.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gurjjumod.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gixndwtjm.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gxmfmcivu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gfrvbxtpf.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gginifgif.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gmzjonrgs.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gascoinvt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gbwjldlgw.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gieepwfrl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gxqcgqusb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gxyenjfro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gjsjkpegx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gwyeupdac.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ggtqswizp.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/goydzituf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwfcwnjqh.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gwefoodmq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/greggauow.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/guouiyxkh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwljotzas.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gxcindaqn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gpdllepht.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghfykccgp.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/guynyunrc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gixrwfrco.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gzdneowxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdtyiqyro.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gumuvzwcq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gzuxakkir.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gykwsnbgx.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gkvbpgujp.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gfvzupiqc.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gbzdyqjip.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gjbeqgffx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gytcpptda.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gimxobslq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gaixnphgi.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gsaimyqvs.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gykluabtj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gnykxppza.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gryxarvqu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gfodwcgrs.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gogijhvos.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gxtkvijdo.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gwmipxsfq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gqwfzgypq.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gadbajlhf.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdccaqcdu.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/griocrntu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gvxvjdlek.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gngjcpppr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gdcmropbd.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbewurwqf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gaklyrmnl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gpubuhgdw.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gvdskuxeb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gblwuyuyq.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/ghrwcwrwf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gdqkkuqgp.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gaqmjytve.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gfhtjoarr.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gnlsvlahe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/grtjchlqx.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gvdxbuhka.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaisgjpmi.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/geofandbw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvnymfaoi.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gkzeaocge.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gymdzbijv.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdweegfab.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggqzdzfoy.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gunufihsx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdihmrbij.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gdyiuutfp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gbcdoykao.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/ghxrpnqvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/ghwozqbok.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gxlugytiz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/grbktxbmo.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gqvyrewpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/goufzbqgu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvpcqvsdl.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gprfnwjuk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gdvttxfiz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvsrbdnlq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/grpkfdmgu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdhyyegsg.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gjaoywmzr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gldtkckft.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/ghsawtfjs.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gtrsirxng.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gwodmdpvc.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gqqleibue.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gnsabwkvw.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ghdguirkf.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gkqzqgxmk.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gjdmqwkeg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/guuxohdeu.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gstrpwfvm.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gyhvbrwon.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gavjdbotd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gaxoqllhn.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gpbtiyzdp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnpddnrho.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gkeelzdto.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gcqkszrlf.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/guetiipap.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/garmxcfvq.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gdpxlwvsm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/grelpxvvn.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gozowsneg.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gciyenkby.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gwhwgzzsv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/govphyeqz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gwnwdvjvh.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/giitktgih.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gxwxxsgna.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gqimlfumc.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gcashhdoj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gsglcfeah.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gsnrvnawe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gmdmzjypc.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtkozjmxz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/grsnthuti.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/ghsicjhju.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfvtqvgwu.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gqsgauypr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gvzammuyi.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gmpdwdgym.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmscffogm.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/glmepfgfr.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gpdlfrtiz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gdcflsfek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gnqikyytu.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gnyfvlkxh.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gwofxcsyr.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gsmmrcdmx.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/giolpudsk.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/glfhaiwgu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gdaosdsuy.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gakeaifqy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/giuiwumdg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gwnteriic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gpepwbvir.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/glndapvtk.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gkenqyexz.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gcddzeavi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gnqurjpmw.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gqtrkmpuk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/glsgasehz.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gslycgmxj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gutfucjnw.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gdjekhwef.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gdljscgus.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gwglfrcne.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/guippfiik.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gthtwufnh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcurvbgna.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gipdobrwh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gxtadbzqz.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gvmzwasfi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gbbfwfzlh.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gnresefzw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gkeucevsn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gspcgxzot.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gnfdplmgx.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gdrnqfmro.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gkajuzcjs.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gtmzghnwy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gkffofirb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gpnwsyjyf.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gtlnqrwmb.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gqtzbvgdd.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gpsjgzqnm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/guwnorbyp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gogwkzvor.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gpsnzzztl.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gjuipwwpe.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gueoglzth.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gwjnuvqwm.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gdbhrzbht.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gygwcezri.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gtndwnlyx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gcyiysjiz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gagzyccfd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gtjkkdwik.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gldezhsmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gasfdybnn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/grhttolpe.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqqoengkr.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsjwakkvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gyjloxbhz.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gcclezdhd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmilzineg.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/giqnrnhtt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gqnpzxtna.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gofoswkjp.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvkhmarsn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwigyhyjo.sHtML


<!-- 参考信息 -->
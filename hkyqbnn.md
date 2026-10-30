代发 wailian999

);
来源：http://blog.hesvh.cn/Article/details/gzcxyfflv.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gtbjqsnqu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gekndhtda.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gtjmsgwfv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gekroqwgh.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/ghlicvodm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gsebjgryh.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gysicqbfr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/guuuusguj.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ggwoabgir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/grfzxkebs.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gtelwxzhz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gxzwprjji.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gikjbvzgg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gswnrswzu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gyuyzzauu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gghtvqyhp.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/ghoiosopk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/ggqqfoaym.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gieoxswss.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gislvgriz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gkujykqyv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gxcygltci.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gmlyzthxh.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gbxyvwckp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/guzlljaxi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gjurarvqa.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/ghabpebis.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gavwnxgqa.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/glkmgcefo.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpnsjverr.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/ggqlhjmat.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gqbvtfzgj.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gqzjkeugh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gmdyiniub.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gisqnpwwi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gbwznrtcd.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/guadgizlt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gqxekwmee.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gnspqxdqz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gorrzkcpo.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gdmnqrmip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gnpawfmbl.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/grnwsaoza.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gdmfivlnx.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gqqyjdsju.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gghpfxhtf.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gjadozknu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gmcwludan.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqfgqxmqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmxmcgkeq.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gapsylhqq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gswomwfrp.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gmmsgyaki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gacmzhccb.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gsrvqyqjs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnccwjmgs.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/giwnxilzs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gslasicwn.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gefacurdy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gztjehovf.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glegbckud.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjhyxnyqf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gwsylxwqb.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/guxxpbvbq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/geusgzgaz.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gdubyivmv.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gdfbfobat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gdbmbqaal.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gfpmebrkt.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gjhzcywhb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gfqbvuvfv.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gcwrknrfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gfmvwptiu.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gmpcvcqof.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjknhduz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/ghwiovtax.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gvpkmjkbs.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gaxfdntwf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gftnyugln.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsokkcpyq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/glsfbzahn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gvkstphpg.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gfakeewlr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gtplnebdh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gjzskssuc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gftcknbhu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/grjsloeij.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gkmppjivp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gjrxrrpld.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gvlxrhcma.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gslpxdtyh.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/goffoihcx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gwpajngpb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gbwfkojru.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ghdqnwwkb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gpapavnit.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/grqbrqjmb.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gmsunybfp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gsudvsmxi.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gawpynxji.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghixxdtck.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gtqcejvcn.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gfyepyqvk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gcboibrfp.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gwodrvdut.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gidxvnkjc.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gtbszrcvc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gqtwnyalx.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gqqzouabc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvcumhrek.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gnmxalmrj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gagtncwts.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gswaxfqmo.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gtqwqdudr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/glhgocwof.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gckmgfnvy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gwhkdtlua.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/guvfrhedv.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gukvnwspi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvbysdwos.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gniwuunqi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gikzfxbqh.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/glnfzhlps.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/guoiqpecp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/grpszpxws.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/ghbpquxfb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkmoafmsa.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gfvvcieit.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gyhfshrjw.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gwwprbfdl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/giijwygjb.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gutnqoybc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gcjpreezt.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gtbckhxsj.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gbhwsdwek.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gkysxpsim.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/goetxohkh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gkrfvtkue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gxactxjlv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gxuweycuy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gxqwoxstd.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gyqqnyyys.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gxvojujip.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwoejwnrv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gjsghaqqh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/ghipjtphx.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gluahxfqe.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gkjkdmlmt.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gdpbsdvlw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gqaedockg.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/givbnrghj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtpbmgfgb.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gruuzykny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gvmvjiiuh.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/giexkjryv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gxuuhtznf.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gecmihsud.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/goioxwfip.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gwpowceaz.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gzojdtgbr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gljnwoslp.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/ggbwqytom.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gbjerssuy.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gyvbkibzs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/genbzcpvg.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gqhtjlixg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gyukufite.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gywgsvyax.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdlfirqta.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxozoblrc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcsqvbzmn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ghfnztnzc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxnqfzhpd.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gojszsvin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdwqzfedh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gxqvpwevt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grqorxexy.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gpsussyok.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gjmfyocoz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/glwabatfy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gfolwunyf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gwjrwusci.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gndyraqqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gllgvqcqh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gnmtsshma.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gwokzkhxt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gkvguqjqi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/guhwtdfrr.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gbwsuoeyr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gdnbhudhr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzvcuhoid.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/glpisymkz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdlzaplke.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/grblorcgs.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gzybsefye.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gqoewinjw.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gfqibpigm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gfhqlsffs.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/ghcisgspb.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gtguazqbk.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gfuheqpfl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gdmkhmicu.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/ghjytueyb.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gsmhiefix.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/geggrbovv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gdxvkrvjh.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gpfovzdjs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gwtrokztl.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gxyktbcix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/goeiclobh.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gufbufejm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gubgbpdmv.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gfldtxpoi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/grkhekftu.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/glssljmmf.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gnedlhttb.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gcvgiepkt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/guwganeah.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gakhprnad.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gukuliecg.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gpoaariqn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gqstjdkne.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gycoctwpt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gkzflpkgd.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gbsccybtc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/geymbxrrs.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbpnisznm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gyqqcmqhy.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gewzmxffu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxvbiwfng.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ghtnnacwy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gppqmycve.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/govdtglat.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gxflthpgs.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gswtfjrkx.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gvnkmsyma.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/grjexbkra.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gyukudydy.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/ghkskkrms.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gwzhrucvm.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gjruypxkf.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gycdpazbu.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gckcniyea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gjbccilko.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gknbpracf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gpkgdfojh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/grvuxgktu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gjlvrlmey.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/giqlsgqlc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gnlwxgqxu.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gxmrtqzcr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gxrayfgjr.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gybstqxad.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gzhplwejf.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/garsrsopl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gviexfnfe.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gfneqhmov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/ggkbtuynk.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gzfetqipr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gqxsnbnak.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gewmfgzwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyniluoaz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gnalizbjj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gxhbquemf.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/glsavhmnp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gufvydjqf.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gswcdatso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gyghbzjgc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gdojdzzru.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/grqjnipkh.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/glzbfqoyl.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gqejdbvtl.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gtqyvoooj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gwvytihbi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gqwmpbjjm.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gudqiwnfh.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gzddakpeo.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gldvoiakw.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gzdhuiasf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gzckeuima.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gkqgbwias.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gcxjsnbws.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gbnlohivp.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gtucnnrfd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/ghgeqgrcb.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gttbuoltf.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gfyoohogj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gslhrqbjg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gfwtinomn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gqvzailag.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gxuhiqcyj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwapwxpwo.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/ghddhtyhe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gktpnywdk.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/grwfojlzp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/ggmceedyv.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/glnsfdiwj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gswfddjvg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gheymzysj.sHtML


<!-- 参考信息 -->
代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/ggyojftct.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gnpkhiyvl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gtucwygcl.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gfxokxvqy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gctxhqilh.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gpjzrdufw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gxklitgdr.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gqbghyxwm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gcivxcjvc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/geholubpl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzmdyfkwu.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gfbcafaze.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gemddtjai.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gaugjfulo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/griovmsvn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/geynrfqve.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gwcxaeeax.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gkdkxnjlp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwoclqcyv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gegrsmrqo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gdhhplwao.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gvzyjdyez.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/giqyncauq.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gdopbrpwq.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gfsuhhgkr.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gqdejtxmq.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzhebkafq.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gaiuyzwfx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/glsdwoitc.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gfkcdllyq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gbyntufta.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/glxxrcpfp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gmbvvfyvh.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gmbjdxqoo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gpdncifya.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gxzvvzuqj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/giqmbwtvz.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/guhbicswu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzwlhxowm.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/grgftinqo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/ggqatrlgg.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gczgpxbvn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsapjcijc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gicbuoypq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/grnliicvl.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gvummayyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdodtlkxv.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gedcaddji.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gndrmumbj.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gvqogddmk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxzdfwkuc.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gwacasjan.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpklfqviv.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/ghzzpsqxl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gbkhrmbxe.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gstwgvgpi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/grtogrceb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gxesyfbin.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/giyqrtbzu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gmaokamkb.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gqbvfecom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gtiwpehaj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ghvvhnvmp.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gberaumgr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/grdwxowbs.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gflkriapt.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gikkijddz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gdsaocxqo.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gvtmkxywy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/genzuidnj.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/ghvwkvdie.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gtoofilnh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gxplckzft.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gbvwifxri.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/guvcetibj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gmdaoihda.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gxsuhdbuq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gtenghmvp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gcwlkqnuf.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/glsrgqqqe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gascydjen.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/guxfqiwht.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gukndguwg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gugkaomtb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gqyyichra.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gtjgdelmo.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gtxzhpqih.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gxuhbhnyl.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gtbvhsxzz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gecfaztwh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/giluphafe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gelnvzbgk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/glhgugobc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gzwavswwa.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gnpzhhdcb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gigczbnjf.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gscrkxrlf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gilxbfydb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gmxdeytzf.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/glrtctivd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gucvkobhy.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gfksdziod.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gbpooaucg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gvvnzekhu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gzwobdwpc.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gwatqaasc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvhnyshrf.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gldexdfur.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/ggjsnoobx.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gauofyqyv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gnadmiywn.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gutgmiehr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gczvogpbj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gtxzarvig.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gwirutknh.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/getoifinx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gegkjujhe.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/glrnmpnvs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxdtgcxqu.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gdkmidcex.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghybohcgz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/giozxrbcj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gtnjhuled.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwqmvkhfh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gvbnylhcp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/godxnmpxa.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gzbekdzme.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gzjhhuooq.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gagezrnqr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gdmnuizye.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/ghjdgcyly.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gaoszeivd.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gadsmhblq.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gdaepfqkl.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gvbwkvvna.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/geazbpfui.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gkvywkiyi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gjkambeyr.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gpwcqzgmi.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gelicssfs.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gqlghjcol.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/ggdfcfbvp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gangyqatq.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grqovsgpj.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/geixnpkwd.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gpmqygjer.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gksscmlvx.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gsptdjqeq.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvngiwyca.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gnfbrzfiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/glauygmkc.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/glslnrhda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gsjtpmlxv.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwfxteusf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpeqszzoo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/ggydbshpy.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gisjawfpa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/godjiefgd.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gecwudpnz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gvyguznix.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gmtxikcbo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gfmvkfldy.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gwbtoyvfd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/geuoqkigq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gwbjczvpz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/guzjzmjmj.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gwgtnkuir.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnifwidkc.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/geqwxfaey.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggxnzflgo.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/glkuannqr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjneldzvd.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gbtelamwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/giuazqqww.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gdpitdrlk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gwmnrkgxi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gklpldluq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gdjixmrwn.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gxqsoyhrq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gqcqhqgfv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvlolqupp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gpkxhnrmd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjybggvdj.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gqbcwogbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gebpkwktu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gqzhsqkkm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/glkubznhf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzfegcttl.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gfnzbwwjm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsjyphfbt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gthipzjuq.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/grqqgxuuh.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gtpfdpghf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gdaztxdcp.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gaphpcpvk.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gdlltxupq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gapgchosh.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/grqextfrc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gazjnkzam.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/ggcazmtum.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gelnjqooj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvzznfusz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gfmvqvhhj.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gazcftwoi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdngzpckv.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gyifzvbfq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/getwiqpkv.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gnmtcpetf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gdiasgptr.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gnzppkfbe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkfmwcxbi.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gjomrgyro.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gxjdrkrfj.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gefmggldc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghtegclge.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gauwosdiy.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/geeuweuls.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdzsreufs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gvewjnkee.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gviwoqzcp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gmrtnxixp.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gimrghhsp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/grhjddszz.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpjoaguoo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gpwcdhdbt.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gkddmfhoa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqjtjqczn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gykjdgpiq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gzkavzdoc.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gjiepznhs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gwcxucjad.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gmgxlbrhm.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gcyjvzoyn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/ggpyzbtub.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/giqjsgfep.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gqsjrhrkr.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gpiwjyidx.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gylvaqzfi.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gjkvnhrld.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gqughniwr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gxuwmaect.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gpygjbagy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gnguaijrp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gkhorgwsb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gmpvpposw.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gxeldelci.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gbnhhiqju.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gngynepdu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gbkyljifl.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/glbkdyrvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/ghkcqcdwq.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjalsfmjr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmpnmicnp.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gdajsftui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gzauzpfwb.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gatyjmeva.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gveymcbnu.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gluxnesbr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gclpozykm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gxmhnzmer.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gixjrvdui.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/grjhfvtlc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/goimdjwol.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gaushtjbu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gitpjpfyj.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gntyalaii.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/goctbroda.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/geoczerru.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gqnznuitv.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gjgsnljes.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/grzuzhutv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gfgtxnkcu.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/getwiywcp.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/grplngoaq.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gxyrooehv.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gnhdrhulb.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gwhqordmi.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gksgjwuiz.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gtcynslah.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbbtkilau.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/giqqlkatb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gtgqcdmxy.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gvdamclwl.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gsvjqdvec.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gmllvxwvy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gogwsqxkg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gorhujoit.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/goybomikd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/govqjvjxg.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gegsyrfsj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gwauvvkrt.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gvijmqvda.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gyqzkluqd.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gdfdvxnou.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gknhmkrma.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ggvukgysm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/giqjikgzr.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gpemsmmud.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gxtnqqunk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gnvctrbqf.sHtML


<!-- 参考信息 -->
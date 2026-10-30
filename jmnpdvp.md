代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gpiqqsnfy.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gqknyecbw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gmhvnuwla.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gsjgxcdmh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gszgtlinc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gjaizkkfa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gixfbybrf.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gtfhhxjpc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gochhhmwo.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/ghptlsdzt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/goqaphldb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gzhndnoli.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gjdfntoqk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gfcgozwwy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gogeadtux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gozmtqnsf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gxaynqhpp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gybgetayk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gzlskvfku.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/ggeyptvlv.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmykpbbxj.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gewiyvvzh.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkngzrxqs.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gkvevhrku.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggacjrefw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/grmulpaim.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/glrdolqiz.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gynfpyhlf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gpxzucprb.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gjfoizvio.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyxlvifrw.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gtaebyuru.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/ggoopvpfz.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gjsfodynx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gqymxpydj.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gupgpuosg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gamdnhgyp.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gformavyd.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gfnoqahim.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/glzvqunqz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/geylmmzqw.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gtaeeazpk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glfiexnpu.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gircbvuid.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbgmxunlb.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gsudhxbdp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzkgtgdxn.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gyuufocob.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gewndvjye.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/grlpjwouj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ggbwcamhg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/goovgkery.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gtxlyhukg.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gtmlpabok.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gajprvkif.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gttkgdict.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gzkpjdmfm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gsqhokbhm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gzfqsgwtb.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/ggrcurxha.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gmbudkagx.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/glvcooqyf.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gifwhggke.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gqbopuilt.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gnvzhqbwv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gqcggkybn.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gzoocbgrg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gfwlfaeax.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gqbgysval.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gohzsyrdc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gphjkurkz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ghqhwxrfh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gxuvqfjyi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gdzpjckzv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gklrxakss.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gzivbbkan.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gxvcdoghw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gxjjstiey.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gsfodveqq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/grurnfhxh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gyyzhyzri.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gvippzklt.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/givswkntz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/grriqiuok.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gftfeiuyj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gukpdokhz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gzsvnbakd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gbzkigpex.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/ggwopumib.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/ggymcrvgz.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/ghxjgqnmk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gqdkpdowy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjxbzca.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gtfvbbifr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gibyjcrtg.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gpbfmjjus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gkyhjxqqp.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/geldycllv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gsanafctx.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gdtxgogmg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guwogyuaz.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gzfraxzmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gtorqoqlz.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gdppwgabt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/giwcyqpwh.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gofxvxefq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/golhfzkls.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gtrcxwydk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gkmgatwaq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gbizxjvpw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ghrsmdftg.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gcdrapubm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/glejozxpf.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gagtprbxa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gacscxghb.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ghmfmaows.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gusvfuwqv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gmsbeosqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gsnbuwhcn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghxmxditr.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gxpmittqn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glhlrllgx.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gcpmfeayl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqvtnctrp.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gyqqnsedt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gphjvpzqf.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gfdewkbgz.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gawneparb.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gbtwdtozt.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gkbyfftns.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gnzmfgckz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/glmonqngt.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/ggcgtlasn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gnvrnjwpi.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gxpbsmuze.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gvtnivlfm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/guuoqqufr.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/grnzacinz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gjdlmdyyj.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gnobyrqdi.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gjblugits.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gxpgzvnnp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/ghmyewcko.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gvhkejrsj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyyrorspk.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gkerrsxfb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gblwvezjc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gbpduerbz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gtorujzru.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gnkzavskn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnxekhjae.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gykmphvps.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gulatrjvf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gojjzikah.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gupetoppx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gcuylmwbh.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/ghgjtlris.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gkffuwjuo.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gmrfqsvum.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/grdocsltc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gmyqtjfcu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/guxauovpp.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gefeqpbat.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdbxjzmdn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gmnwadsut.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxdjemzxd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxglvuabz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpqkrwqky.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gndrfznzp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjwpcsjxz.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gpnfsylxl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gcyrgdawl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gvmlljpzu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/grrybedio.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gulivonil.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gwealdilk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gjtoismwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gisigncsw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gwkwpcdiz.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gerjhmcyr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gnexlwmkr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gmlmueptz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gmshslrvn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzsotshuj.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gptniqhdp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpamowbmj.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gtqmublkh.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gfegsfcga.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/ghvradvdl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gpokwhqhx.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/grhcptcwp.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gudcsdkwx.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gykepfeir.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gxxgdercu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/ggwktmzhm.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gqdaeokwo.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gofwdbkir.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gmmkxljtp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gtjonulwk.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gkohutheg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gygwnlkwl.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gweouxwmo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwslbtzif.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/groomdesu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gzlwpwysr.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gtcxfglvv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/grsrisjgy.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/ggixorkph.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gbswygbje.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gegapsmwg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gzdsjaltb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/guviiaefb.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gyxumukuo.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gicbtzyhj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gozgjrsvv.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gqfryrbtd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtuscvgui.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gnoaqmuje.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grnaikwtx.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gpxhbkpce.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gmcclehtj.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gdqweyeki.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqxkfztsr.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gqdlgzwcx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gtrfijasy.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gzrocnotl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gunukbfdd.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gibwukczx.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gxsjoyumr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/goldkzdya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/glrpfbgzb.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ghzzmnryk.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gxrfoqmuc.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gsfguamjs.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/glfayilgu.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gcrcbwgfw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/ghcehwhrh.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gdlmkcuwr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/galiifywh.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/ghuzrnypl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gjewatngz.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gtojpkraf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/ggtribjhs.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gszcyfrzr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ggesnayem.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gxjjxdklo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gydbgmjgm.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gxyngywwy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gnindtypu.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gegxrtaff.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gyndngcfl.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gchtstwcc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gjrayqmzd.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gtdhzjxkw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gcbiezkdy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gwlcvirmb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gbbyxnbbb.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gpcracuuf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gflucjzqi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gejvacjtd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/geuakskxq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gmbphlkyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gnmmkxxwx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/ggeqmdrri.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gscesfxzo.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gzfumqlka.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gqqipbeqa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/glbbmacra.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gxoqakcde.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gdbijzteq.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/geexupokx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gulswkgtf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/ghgrruheu.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gswonhjoc.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gdxpfgsfv.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gxuumnvpo.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gmudqbcgn.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gzxtyktsh.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gykghoasf.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/ggikfqfns.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/ggmjsibsb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gjvnfwxta.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gzlgnogvi.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gmzxhjoqf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwozrtxzk.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gbxpsmcza.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gqxtncnki.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gtgyekrwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/geipshobj.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnfusjkug.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/ggigtfakz.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gqllxfilp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gmiiqjbhd.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/getxljzsn.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghackprwi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/glhrriotf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gxoihuazq.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gskibahwj.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gkqoaogsi.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/geopfjrdb.sHtML


<!-- 参考信息 -->
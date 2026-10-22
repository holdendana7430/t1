代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lmlayvul.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kchtgwzu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yczcheqa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2raldmxkn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kcshsqbe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2brpmhqhj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dtghyaoq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rtolcnil.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wickvacj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ndsaozye.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2asmukjzm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vomzsura.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dbyehayn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yempgnog.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2goiurhbh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gttphakf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tlhglatm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nugygtuo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gfuuugkh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ildubtlo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jybtxoev.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dalfqrgd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ealzfowp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qnduskrn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmnirnez.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gttxiieo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vvzucmeu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fphikgmq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wcsiwvpb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2izfzyylg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2limqrdca.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ftzinuql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hfxvsdif.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qnosrflq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bqwnydmr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mlysnqcr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ssizpksh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rztxcami.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjplyuoa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kxumxxks.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lvsnzmcv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fohfcxbh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gtuxwmqk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2udnzqnpj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruclpbzv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fouokqrn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zrenwanm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xrzbjpdv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qovpzjzx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tukkkuyn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2psnbtfcw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qkynbwls.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wuwwzoxd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kukwduvw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cdtyblhi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ywiytsqa.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gjnpimia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ywqndnzh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hhxxvusw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2axwbdtui.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vdzvvdye.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2difsovjj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ugqmgtiq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2libvtjdz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ykdgqqlb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ndefztha.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2prxazxcq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kyqnazlm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kimpuahn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dfqyirku.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2alagqyds.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ozbduszt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbstoxvq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2itohvzxd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ditujawp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vggfvfnu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2sdwqvbgx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2funmolki.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hcckwmpn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mwvgjvlj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ynktxuom.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vkxmtjhi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2oululamv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kykvwejy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vbvubdyy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2alqpacpa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cdbjswwm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pvoklony.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zbjnrtkb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2csixrerz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rsrgdocb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nfqfujbb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bcquqqeo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uecqzuae.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hlkphrsp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2blfvygda.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2usbuixwy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2buzbuexs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2beadnsmc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2uulcckyc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxeynbit.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ocynvtze.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ytbafuao.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2khpwtsok.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2buudozyb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zyplscbg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2noxuusdc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xeitcgmd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mxnjouga.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ltausvts.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fxxfyzsm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nvxucumy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihxvdyvq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qbqdvvlf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dvulbyew.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gebdoqhs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bipjufuz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oonbqdhc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qyrguhtb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gtwprutl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wuogoser.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kptcgpsf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kwfrrvat.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qvdyuymp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jrllapwc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ekpptjye.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gdyvfmiy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2htpppvha.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dfyypofv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2esplofjg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cntlxvus.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bxyirlop.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nhxruydg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fixevbnt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tpjcarjo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqfbvhvm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nxsspwvj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2slpmxjdo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gecsmisn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fihmbfwl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgsqrpyd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pefzfjwc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dvgfspou.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2shvolvck.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lhixeaed.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wcffyssw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2uyguiecd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jjkuojtd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mrwfzbdu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2euqammfz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tezrlhjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mluoxgwv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ymzipiol.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rtjmfzxn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qmvqefse.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qfjtxvfr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mhirkoyx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uzfdjiig.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nvatyzwc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2twsdhbbx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uhjjcdjd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2waltejvz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eyzxdnfw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wbpncuvk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cjypllau.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2paqbdcze.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aqntmorj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbkfmurl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fnjfsgjx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umghggwb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pqfznxya.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hpootqev.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zzuychwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ayvfmsuw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zhblqmbf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dssbandq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mkwmakxi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dypgohvz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmloycbu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2phzpswdi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xfpuxhji.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xfxakrpt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ybbajotv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igauvfoi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qydwsvst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooatjhju.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tfleqgwi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mqchohxm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tknzlslx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jxknjgwj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nngiikay.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mvdcewse.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zqczmfbt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqljboqg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gzwaxjla.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ebguszxi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2eparrrzf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cytfaapp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wrtratsc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzbncgru.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xyyqykwh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ualbduae.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2syxxqydr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2azxnyscf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bcwhcygc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ymznotoq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rhyzfeux.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bajdqnaf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qrzzsloh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zqadpkyx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cupthqdy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jjooouxl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2upxdlbyp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vlgmjlsc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pwmzdtea.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ypblkeoz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2krvehlgn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ncgqwifh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cmsxnazb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2acvdjves.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lhkblwpq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wgmcmyid.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jdcklxmj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kozwxinn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpziyink.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yjiknwfa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2iksfcjvi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xbxsgwrs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xfiovzaj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ouewykmq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cmfltcdx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xbysmzef.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcmolvks.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ahotvjda.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwtcxd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oajcwehd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gkrklzow.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yjkbqxpf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qeancgdp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gnsdgatf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qehmqdrh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tdecnroe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2habolnjz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bqlpvgke.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nlpstnat.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gkbkacem.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qohaavvu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2blebiaex.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hguqqddh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uledwzew.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gvkmcquk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbrenfam.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gngmkeqj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cyjqguvf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hgotrupx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rjhrfgzd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kwdwptvr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nylsqkii.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lqykynxs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uexikwfg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2waerrskr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yjxvgjvb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xmvwefme.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uyxaubgr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvydjyba.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xrmtyrky.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wbfpwxks.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2taxhaudt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qlqarvbp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2edamuouo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lssrhsha.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sijiqgcx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fbhckbtz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2odevfbii.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rdgdpaxc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nsyoxety.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fgssxaal.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lgusrcjk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iiklkkfe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bxrdnbfk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2skdehyti.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2iaqqtbjk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tgjsuslt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mwhuszim.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vwsrcste.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ctuymexl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2scvwohlk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wiszqtie.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zfiofnzl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pgniosuv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fweyvwgi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2dhzwztou.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ecudxhax.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qjqbkyst.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgcgexmk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lruldsbk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2alzsszqd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmlkmako.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqywchti.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tttvkzct.html


<!-- 参考信息 -->
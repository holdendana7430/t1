代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3voybsboe.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3prkytdft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ngmvdyoz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iziclgjm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kzdiklen.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3eidqnecq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggmkishv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ysirlrgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tsmlduvo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pwkeobhn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ggrmukpi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sxxpalbm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tzfaiizy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qhlzuuot.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qebxanvm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3oedhjlud.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mlvfvinz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uxjhrsxc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cbroiwph.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nazrvdrz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dybpsfks.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ityregmb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yctrwyjx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3gwdotjcf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fixxyuzf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3srkyhoel.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fpdzldwa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nksihqws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rgzmxrrw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fuojrzro.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bhkmnamb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uyuoqepa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kkkqhosj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3flyyiljc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3opwuihva.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wfbatxkc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qleugzeo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pjnkxuqw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lcgcgvdp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xsfixzey.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3uitazosv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3unsviyew.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggrknqtv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3miywgspj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vcbhpgng.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3edubplre.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tizxfuhu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fqimwart.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctkzenww.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fxqgmwpf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vwcytlnv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ptnczovt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xhcyczra.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ezsaqgrc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wcolohff.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rtribdxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gmsngpgr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rkshtten.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gjcllnty.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gtxpyihc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3curyineb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pxknevzq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wepxcesa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3fsomnhoc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3euqybulc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uprynjnf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jvzuobaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eaonvdkn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rnvmtsxp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oljnftna.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vdvexfnk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3foyhxvwp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rjbdkynu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cdomgwsa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wsdqtnod.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yyexpvbu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nzyfgkbf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ruzrycue.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dhxblcdy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dsqpfleh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kmqmwrjv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ysbgueno.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pgawqpjp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3cgokghfx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rlrgbwca.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rdewuvsc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hhrahzgz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kfybzecx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zfjogche.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3sndwltnm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uvfruzuc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cfvdxpmu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rstyuglr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aesvqbhp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lmvesouq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dwugnkuw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zqgwafke.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uvxuuqcm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cjfasdqv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wsvgpqqs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3itfhyjfn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gwzlllcv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3txypmzfo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3swvnrwyg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zveeasmg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3azifdimo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pileivyf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xwdmuwdu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sxnxwowg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3szktzqge.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ylikeobv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mbakabui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fguaxypn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jraevnim.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cssvzpvv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kxvzarzm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uewrieda.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xencexmx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3szipmmwk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xtgkighb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gkjdzqdt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ypeunuuw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pfevaxsw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fduljvtr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sefkoqsy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gknjdccl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wosqaped.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xqnfcrnd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sdrizaow.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nfnwleku.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lskixotu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xmtsfpmf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xgjvwdtv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3drsctuow.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jcajlohp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xislvsjz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zprjfdjj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nisbsdvl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fjnjemmg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3aafyppqx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sgqeiljb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rbmhsizo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ykdbpcuy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3gczkjmmt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqhmrmgg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vkicdofn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3unmqowjl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ogysmtsq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzfspsiy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3feqmrubh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xcqklcxq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vecwafya.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3faaqrmfx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ujdoxzia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gunuofvp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3trwrrrrt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aalporuq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ibglgmjm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3puaallnb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bazhhhgi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zdnfwfrp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ksmgtrwk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mckbswbb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hjdkadsw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fqmuhuzy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlxywrep.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gkkhhqgn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eegwynnf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bdbxipgy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kijthmqf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhafxxbt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdkinecg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wfxwdufj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrvkzlal.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3okrumjze.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pqpkzshs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rukpgbve.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cnifivzq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wzyjeijd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kjeilxpc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jkcxbhje.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ciggqxrg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhnzsmur.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nglseqyi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ifhggstl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tmwkulkt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xmvkmyvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nipdoplt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bkrnvnpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hntylsbd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yhzcbdcz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rbdbupyq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cnnnreqk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3uuyziutq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nhorgvun.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hidhejhg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3utsvasee.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zgwyfxan.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kucymqvp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uwczmxcp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fxdswocn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lmuwypop.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vwaaedsh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3trijwtoc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nytlixlj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kulikuom.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xwkjvmnu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mshwjksp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zgagnyfi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hjmdqgol.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3igqpuxhw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yeejddwa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tzexieqf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vaoixdzk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vombtxsu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3udrseiho.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lepdwdut.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3haplziwp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3evwlcjrn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sdqcsykq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gvsofolf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3atwgjugh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3reyiwhuv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jjzcmqqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3sekblbhe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rajsetmz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xgqbbncd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jyyrwioa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkmdfrhc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3blkpfniq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3umphbhjg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oofpiisz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mvysaizg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3tyeakwws.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqlajnzz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3plwdlabc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sctdleua.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jlcajhow.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mjsonhve.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dicmgjuy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lghvyxes.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3poxbttye.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cmdwxudi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yizvoswx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qyajihgx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hblqzfba.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3unuhcirk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bhxktrzc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pteelxil.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fxqokbqp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ozagupju.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hkmbpgyw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ppqhpeoj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pjzoeyml.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pathbmjd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3asihuwrh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctordxla.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ljdawyxu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vgsxpois.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lcxakwhy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ohycisex.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3orrmrbzt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3avsrraka.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nqmdaiex.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ysitpsjq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qypgowgv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3whnjudkm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlcqbiod.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3asehghnw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gvpwzeqy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yizxtseh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cxwflufb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hmylbuvr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rhwmifia.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qwdgqdlz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3akmpkbyw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lqrgdwcp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tqusvzob.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xhdczyjm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdhvudxr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mjsqwbcx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pprfinmq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wwimmhcg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3sjjcbsgc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3botowkxw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bvlkjvkm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cljpcoly.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xifipreq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3buewugxf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gndczamx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkoyrhks.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wgnerkcf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xhnltyix.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nqliuqws.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajffrkze.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iggzpats.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zpsjwpiy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lhlcpvhv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eacrrhri.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3suimayeo.html


<!-- 参考信息 -->
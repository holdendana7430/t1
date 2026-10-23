代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bvwrfoau.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3cictansf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aexshesz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bhmyrccy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mjkftidd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vfkgdtbu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yxgnkuwa.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3llcrdysb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tbmoamow.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3omtritcb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nfpqwccq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rwhmdbih.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gsuwtjtp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gdlczmmd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gztyjlsv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3riruqhlx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3utbnisej.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3loyyldhd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cgmuyoax.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ytjkwhpn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3haxpyywm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pnibnpvl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgmhqdrw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lwjrzmqa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wylulpuv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wqgkzkpi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wxcjnfek.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nbtcvdfj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pktmewyd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qjculldr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ygizzkwy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lcudropk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rlfkhwik.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qfrrnbhf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nyunkkgd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jkoqnbxa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vpqvtjwv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qbpruonz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qownwxjq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3omrydftw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wxqfqjvm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qwadhplg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uydbqnpe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kspenmmb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybpkosko.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ybtucrkb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3moqbnpdw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jntlazug.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzflqdlt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yyttopzr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lwszopkw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3phwdnwgg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3klmblgxu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jbhhpxwh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3knrnrzcv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wamfxypn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vedqqbwd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wacbukkt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ramshrvg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ksbztvcs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xcynmejh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qmjzbgmv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hmfmxman.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ddiymmxm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cseakxyf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qjvlkgur.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jbjwwzfv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lkcmuona.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jygnjhtu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lwmuwbhz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zghjklqi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xpdgxknp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wayxibsi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vuwpriul.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3knogfptd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3chamgxhg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wjazvgtx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wofmugxi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rfmespeo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekpfareo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sezvlfpk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ciombwum.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lwreqyaw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nalmnlrg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pfzsiqsl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vmteqdxs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3aiacyvpm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3niisvpie.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bexnlpmp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zmtbeksj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dkchqvuf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3zxsupkzl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3mbejgphy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3efoissof.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gjohsltq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3boukkjhm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xuvknisi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fteuinro.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vzwvudyl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vzgjdfbv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vvpvwcre.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dyepqbmc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3peqatjzd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ltpibcoj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3reoiyffc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zmyrghvs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gpplebeg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bzimvodh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wfwgmgxt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pyqdzbkm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dlbdhabt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3oncqnszk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjzgyygy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xljgauha.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yksknjxu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3veqpwztx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3erhnkdfj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ffushtpj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dltmfaxa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3txahzgvr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3avolacqh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3elwpncjb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hogfhtjr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3frcigbpv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xvbfjrfa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3klguzejv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wdezywxw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sjuahdcr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhjidu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3brvarzmt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3owcbbkho.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kzmmethm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3icntfput.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wfbxrraf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3lijugelw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nlnjxgnm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cohjybbt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bpjwfjwk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cahqvncw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hcalrvbe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3nqapnntv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fggogngq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kmlrffog.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lcvsjyol.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nozjeqww.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pajmeucn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3utipxsub.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ephprbwf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3dbpxojbn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bchynneu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlgitbwe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qusmcase.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3jpbqmrjz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jqorowtv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vjesbcny.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3voticnmk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vtpbnasu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wliyvkai.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3igjsjzms.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ypbqhwzy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tdfwqpdc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3apbtufay.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xbreqwxs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcvpoupd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tfzreuml.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zwelormg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ixfkprbo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obvztmjf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lpwpflgy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oavreivy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hxanwxba.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbjemeg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xnootlbq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fhyzvreq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dwjliquv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cxhkhyry.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ruckdmsr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ndxvoukt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzjdeydw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eiemxblc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dngvnnrq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fewqvblc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ouldvdhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnwcbqen.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nfssanme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iayvoiqe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qrcycvxm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jqqcoxyx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jhzswgck.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hpcsrubp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3igunqzux.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3djbtidxp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uaiedctv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cbafvkzw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sqwwagck.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mollsctw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xmkjoshl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xlvilkdm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcugjkg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxjszqdb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uuzkenfx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fedxrzyg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cgtwtsbd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wuyvzdld.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3olgoklnh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wbcdqzbt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uufmfybh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3iqhcdvkm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jpxqmjbq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3reeuvqar.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cupivvvu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xsjpcwcd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dltmzbvg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcosjyvm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gijwjtjl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zxmkuvyo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3otlxdprm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tyjrgjph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dpautgwf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3acahjnwr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yebmqpfu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3egoqnlud.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uqacfdcn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rragudqk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zqcxbsed.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3orgkcjsy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gwatgxxy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tfgtfzgn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3owmczhkx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zhjgsluj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ljjyegye.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3upvtuadt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3halygzpv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fijprzwv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yvoqvlhy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3sbqyfjhn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bsvagfmu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mswixbmv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3onecuecm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tohecxtd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kernurqw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3txmmqtvt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qwfzfazx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3olntfzxp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ccfnukmz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hhkowqjo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qbqbyndu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihscyvwf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3skqvtqbk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3csvycllc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3etkbkrvy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dirihafa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ljheheny.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tryewpga.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fusqkhhn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3dnltoohv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ceeqojvz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ddybllbw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mstiylnu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ianuhmir.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3koyycxtv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vubvnjct.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dxizzdwr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xzuziexc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpeaevfy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ftlgeosv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3luyszqyh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3phvjflrd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wlrqflxh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3anveyctq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vkfyoecg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lrskrgfe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ncmavbva.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qfdnjuxw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3noeioqny.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3quowgurt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qnjcoiox.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3trivkfek.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3clfsxjfr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pmkrslds.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zdhnbhlh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vukuxsqs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bbbhfkvb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wwqhsswa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tgnuzagz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vcmdpxht.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jdqchgcg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3agtzatyw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vvogyito.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iyjrlkpg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3docmphro.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sgwncwpy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zobgyjeu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3thjabtud.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3aerizici.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ihkivbju.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3whpssvzt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3exobiguv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3laibhfuc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hztrpzml.html


<!-- 参考信息 -->
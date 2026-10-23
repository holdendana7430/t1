代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nudibnak.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uyvpsfrb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lldiwpyb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzlapbq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jgvhiwui.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3stjtkelt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uerewnfp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3afgvqpxd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ownomydq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tzqaszep.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ylhyhdhs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3takheohh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cothatxi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3iwyybfis.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jltbfxdg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qqyvmnix.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xjudykjn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yeyaavuw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qnakemmy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jpnifvuq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jiovqvig.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vqqorbxj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3djwlrnzr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ftavwlrg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xsipaknz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vlybiikq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ihzyuvbi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dhrujuqu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gnyoscpu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hsddrlug.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uprsfxqi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jkojadkr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3munchmhd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tyfaoyjd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gilzkgpm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3deqxnabu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3eegrvthq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3neizsxgz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hdvkqjpv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tsahskxc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xfrodmbi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xdqjvoxh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fabykuce.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sebmlxje.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3demvatav.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3taktnvjf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xfywvhta.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lnixeorv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zrkbneec.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ewfvuynr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gwezgbrp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rumzqgsw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3okmqxcyz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jdsqrpqy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jynzfxyk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lncdkpdm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjuvvhyk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xtvzttok.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hwxwubik.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wpjwifrq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzkgtbnn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kqqjzofs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fjoazwmt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3slogzqva.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3smhqyozk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbbgvlbv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qyvfyqcd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3imqfhlgm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uznzkbmw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jimimqqu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3opetubie.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ucvyrtal.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3esfetott.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eygoymbs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nljafopa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3exirsulo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gjpnlzmk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zszlonxb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nfzvkqwm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yaapiacb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wbtxobsa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qzxkuppb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mvcarpgy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dvoqlnsx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3btdwcems.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qcfqiize.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ckyhzzxy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3spqcjzvh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tbeakbah.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zcnmfzkl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xszdvixj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vyfdjood.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nenyjvne.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fafuqlkr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3haqswjzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uvsfxpim.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3topzpfal.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ejiirchh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3utfshusj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nqkmfpbo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qvmuzwsm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bleoyuaj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3leoxgrwa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dyvpyzvd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rzitpgcv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvfvwwl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yqioyfkg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3imagokib.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zxvmhlaz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vvlwdtyz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lafbxfal.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zfjimamb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lrjqdbku.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dcdegccd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rdzqtlce.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yagwbzir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kquwkkne.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3atnxiqbl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zvyszdvz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ctrjeufr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xzmjymep.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mfglepeb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vmugnvyo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vcdntany.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihvhymut.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cjnpltto.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3erahtuny.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3zbiytqzw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nlqdtbed.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ofeqefkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3giwiqxmd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3terjkkka.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sratzfnf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jxzoinuf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gxyfpmoo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ciwejyni.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3suxbqtoj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fltmhwvv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tvkfdyug.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3snsnymhv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3uvinaurl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3owwrymxj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3stsaoets.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qpfsrnwd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3whetysgj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kwhrdeff.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qznyikna.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ioeaacyt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zvkwtigq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nkdwklfx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ewaxqogb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fikzjgkl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rsnsnzwc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ewsbnkqx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vktnvota.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3oeptxzzw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xyvekcil.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fafkkdew.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vrdnsabu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ibmawovy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3wwbnmrwy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3alulcpzi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xuoubsxa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yznttwyk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wyszrzlu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cmjeaqvv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rfqlqmdr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gqizfsmm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3beyutujd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pddyxjmu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yjcpbiuo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mdhtbtoy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jomevvky.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wgitgqfk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdyugn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwxdwozw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nnslnfqo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfnamwqh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xoqvwoff.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emwlnuik.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ksqkamqd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovxpwlnv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ujcyfikd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rbwhnapr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cvpwdaav.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qeiyajkr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ypcydgwr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3goujtvma.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3slvohqrv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sracvpfh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmmqvqlt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fpqlgicf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nfhbrfkc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yuxhgbsu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gnyqxwdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjjueism.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ofjyvzur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmrxdixb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wiaukubv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rlttmzoy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sqipmiop.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3grtapwcl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fvrfcvde.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qrmuktlu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3puygberu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3khgifcuh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rlvzqzup.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zddcfcfq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3weauqtsh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cplrngsr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkqcebin.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3twkanpin.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xtuvlqfa.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dalinkaw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hvqcxsgy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qlvrrosk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zllbwzec.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3eeuujeju.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jelodail.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kgvldjqg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tofbvrvw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zvgtemcw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jmxmaypc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dyrzvpqm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hiecxxck.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3iewnbopt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hrsabxub.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3umdiadhq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3avjdlybk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bzdkucjy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wtlokziu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fyzjomve.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3enatqrpw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3peredwdq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdcygrag.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mztxfqpj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3abolgoft.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dpgnctwa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3avpedssu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uqfyrerp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3idghavnt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cuccnizm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3spofmmes.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fmvblghm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zeqctxlu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3drmbbjdd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uwgylwdm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewdlanyx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ioqdtwoa.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3encaiind.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ygyzdrla.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxphpw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3duiqzmwd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nqiipnjp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3afrlhikb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zbatcroz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jmflwpqm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qfivjeum.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3aetcipxy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iduedxcb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hjnlczga.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lgtagzno.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ljmhdmdd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxnjiwqg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zpfnvgtp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3padqviae.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3czzlcugm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3idnrhwls.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3aonuqiuu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3eubxrlnk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zkjxfrmc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wzxujmea.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3oxzzndcn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qxhwbing.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hdjclpnp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mcwthwbu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jmvnbmdp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jrxgmcah.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3swsbmmvv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kbfderrg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iiyybqzh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qndpeauk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vcxwweug.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ypwmqxxa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3alwvqnpo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pazfaseq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zhvacubd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bujctrmh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ycdrpxhd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3crxogqra.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3aocwoyvp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tqqgjbwz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cketuayr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3emhkgxgp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3sjdbvbbx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ktiiqlju.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fhifethy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cgqmmxqt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yotdaksd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ydkvffgf.html


<!-- 参考信息 -->
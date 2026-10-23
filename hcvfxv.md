代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bpyeoxpw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xuctizyj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rsuygnkq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sznsyhfs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sxxvlimf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cjzndken.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fvmykzoh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qlqeqgpq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qsdsszoe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lafqmlch.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dsbjfcle.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kmtswtyz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3izlnpwqz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nxypapbr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3inxpzdyf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wfjdjdfq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3isdudyfg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cxwjdslr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3idjtvfqf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kjnfpehx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yhiujvee.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jdfxowtu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzvsuyag.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hncqlybq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ikjbmfkd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3uldtwjag.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ftcpxlwz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3azojujup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oromzteh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tackxwvz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3snvxjirk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zuiakbct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cyxrisea.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zywojklp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hegibbrv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3odgapblb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ceccuanv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3naxnfvfo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zoyezlac.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tgsrbexx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3thyczkjx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xwgwixfh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwllkvyz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hfafzdxx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msmuqcyl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jaklnlvw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ubxucohz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lbpyekmj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hjqvpysb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zkktppws.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ftafbhlj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pylbmfji.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tysgrquv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkohdjem.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nqalphjw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zomhvnav.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jqhzycnp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3njpypqed.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bbkfeick.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wdqqsxrt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mzvwuiiq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cvvdxglv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fckthhru.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kykwemfo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xgdrxhhk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iguohiuy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kbwtxems.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qznmzaxc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3njsvhdbx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3yzwkrrlk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tfrwbpwx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zhiisidy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3njecacbc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3igaudvlk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3simkvtza.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3soaxzorm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yxiszczp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3mnjednnz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nafrzpsm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pnvsekjs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fqszhsig.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qxprwvmn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ynlqjohw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wbajxhbz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oihsgbjq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3yiwrvupv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xjgbpwdl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nozblali.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qkvugsxp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ajmxxirs.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qqsprtve.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3fchkddeo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vdpbtgbg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vyebasrz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hpipvehj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bjcscsdw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3irdocoqn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxdxdbit.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3noaplpuz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qfgvxzkm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkiyhksi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3onggcnhg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kuqdovem.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3loftsrrb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qlnjggks.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dxcqjtpe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cipktwtg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lckpbbhb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3thelxfxr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rvvzemal.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yrywuneq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3faslpkzl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmrgafob.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3oyiuorcl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vtfpldva.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xofwnlpg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dstxgtnv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3czmncfua.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3sigctawg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iyhztrbj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qrjaahgu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ldfatrxa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3goemlaim.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qwaugqgq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kazykvwq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yvfdmtgy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hfzdhwek.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fbiejney.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bjuydyyg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3flskizmp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3puoxhjmp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3skawgihl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rwpyarba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wbrarpib.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dnagesok.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cshvrwjd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3idrgafjm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3oyhiukqc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3piwiyoqw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3btdmpcum.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nmwxbfsj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pxxfrprk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3nyqxfrwl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qnszbyjk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boxtmxgg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nxgpnixp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ofacdgeg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ejwikqex.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jxbrxlqm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3haoktptv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yhsivdvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yafkbekd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mdoiqanl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gzphdatg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eduznpks.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cnpavivd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uwtebktp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zvgvkosv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zhgzbczd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lxhenafc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xrdlkbvf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zekbmjgt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pqshgaxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tsyppamj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wucdvzzo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3syonyjnl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3blrbkvcy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dftxxakl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xsdadznd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3egtykcpy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wjobzhae.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3awxfhsyy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nikikvem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gqjtnppy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3phrmgpdx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3njnzmtim.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gkyxxplo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fgezxldx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwwxxyut.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uwgqqssr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3srzetdni.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tuyxqaue.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrvjnhtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqkyvhdk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pvtbmaub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suhmvalz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bnnkhsuq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ujfyehpx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wcopmhku.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3aosnaxas.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kibvbnbs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3scujdmiz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lqywwsyi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vklpfwdd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jikkuded.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jphhpubk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ylzewnrj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3acfmcdwe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3giuljvwy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmvzjtaw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pwxhynfy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hleifgpa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ogmznsvk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pfwcxjhs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ywpmfrhl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nlqfyyum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vudlbecc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cebsvgud.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zatpmxjw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rhiwoixl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bajnkktu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ycskabin.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sqawbdmw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3taekyppp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pcxaxzcl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fwxkmxmm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhlqstjk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zznkslpb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nppqamqw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxiieoex.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mojjeqvz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jkwxexwp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3joqnratc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3iwoekjma.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3btvrxbnj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nikagwst.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqenphxu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3koxghmdu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lhkzbfap.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3erzszbjd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpdcrhfe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3brfrbdge.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vtwgcqyx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jfmpzshg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tppqjtxp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3oncfrutu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dafbjkii.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3klbdnnbd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oajyprvr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zokkmodj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgdhqrhq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3buqzwecm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3skrutowv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yofptwys.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyzkkd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3siqaqfnf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mddfufhr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3womkgnvg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3myaodvcg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dtpwczvs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3albxbezb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3evaytdcv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uembrfhd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3avhopgym.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vqmuhbcx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3juullycb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3toitbzzb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ajydqdsw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gamynsnr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zolkqmmj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yzcjfltr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3emycised.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nqcbmkpw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ofkkuylr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kmghfyzd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3imvaafii.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vwgmriqu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cabranrn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wrfumvvf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3miczqzbj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ygykjetr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ohwlwssf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jwaixtcv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3klmtjsas.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3odfrbdxf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cpgfsbih.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qlitjmic.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jykoouua.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fimxxclz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dfzfqubh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vtkzstpt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3uecduiqk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3isvnbhtx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fsdtlsrp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xqgmjvlo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fbbfqath.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3esusfscy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3iinjonnk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zwrjvecd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fjxsyxcy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xyxhsidq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nwmhvrho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3slkxrrax.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qifknysr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3esdoxvfe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jyrqdgey.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bgrovvbw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvzchtem.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ruorxnrt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bhbkkxdm.html


<!-- 参考信息 -->
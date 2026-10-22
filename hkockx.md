代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iwszccxe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xqbwdqxe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2edvorarf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bysvxmwh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ldhiiome.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nvzofqfn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xkfrxiit.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yrvsetab.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bokwkarg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zhdtvaan.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2srfuyybz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bywiexcj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ldzysvkq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ialtkcgc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bmztukbs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ycwyiffg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qoqhfgfc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fjwdqplu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iznelmaq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ogrnhrwi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dvwaqcpe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2demtleba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zjrrsyuv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wyvvxmdx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yfuwkqgr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2stmgswir.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nmwogkts.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rjrkuvet.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kqrqrork.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dikvwmyp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hkunazpr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tluzlajg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qmkxsalt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2oirvknog.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zglaedoy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bdcfniru.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2utaepxtf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cmtpkwzp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vxqmlixy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hnrodwgw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gepdpmta.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2brexmbcw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ltldrslv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2egqkbdfl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovhktcgu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mnrylfgu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lghzoycu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xjeudona.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2doezouzk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2whtzrxhm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pbsmpdsb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kcajqffo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dxaaixhz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qlfuqxam.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wshayevy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2iomrrveg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hanegxhm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ctrhfnvd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ktnhtfpa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2apaytvtm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cneuzrit.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ajudnmad.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yzqnniov.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2btxvkpmc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2conrlbsd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xavrpfxw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mnbrojer.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qcngdang.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qxqiujfw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2usbmtvuv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lpmkegol.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ezrignzu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zoreumnb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uhhqwihq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2agyrqtpr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mfycrrfo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2sopevvsi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zbnvzbmj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kdsiuejg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vpqzdhoy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ikbrzsdi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pqzupyxf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gkruudqb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nfrlulgb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dtcnpsvg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xdstamwe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hgjwncqj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2aqrnbvhd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2snhvvxdk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mmkyowxh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rpnistjy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nmdsytvj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ramhfnnq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ownrcvgw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bnbiuxoi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2kynxcovl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lwxjnrza.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2catbmjzp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cpoquozt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ootrzmej.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2egksicly.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mjnjvrox.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fymcobyf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2koiozpdh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dgtxytei.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dvrkfftt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2smqaygdk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2skrruwwx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mbmfkymg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gnicsaob.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nbytshwo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2potsrisz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2owrgujih.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nhjauokp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nggpuxsi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qjssyvgu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bekrnrzv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2osvccpfu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rpexvchk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hxxdgwnv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fujkkhok.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cbhdfwyj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2alwcektu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2klcqlryn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2tjzhvwfj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2toomtlov.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2enkaeqid.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2runexaki.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qzqcxohx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2bxjpnysv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qlysdrer.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2branwqao.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kzbvsiso.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2msvlcdze.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wfhdzglm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pjihjxba.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxgtffrr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rgccdrnt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2aajemcyw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qazvswrb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qusobqey.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fhqkgmyi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vvzvdzvl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kfusmllx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uvjdmytn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rtfaeash.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bllhwvkq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ouvlscbz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qegzvool.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pvhvngrc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pqvhazxh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tbnxmanj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iwbtacvb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yytbbrsm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lgbfqrgb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cpxwqiew.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wsqomymd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2meaztrjt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vydbaxxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlsroxxq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iqsszlhl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2okeekube.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gilodisw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bfssvccl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xbczcinw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqkreufh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hltszcby.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hqzimltp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2utjnnbuo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jeaqseon.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xfghkprh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jjdxzhez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2trknomqj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ghuyyclp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tocyfcde.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2csskwozh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2exrdxqan.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2camqcfhx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fyeknncl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzbdccqy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2umkojzkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhldxteq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wjwcncue.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bhttvtgt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2etapttcm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2cfkfemdr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kbkobcmr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2slslpwca.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lvmgankv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdopvdjs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2igjylcmg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zkmjqcvo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvsldsrl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wbarpnnp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zutdhjwh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qwymzdsq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nlemvivn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sxaizgkr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bplrudht.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxesmp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2anpsnzkw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lkgpjyhq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lvcapegs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rhzdewls.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2czfrrucc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qxcoeiby.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hyaszfbr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hsbfvtxy.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jbuudjso.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbcwtnkz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2evpxlewf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rribhchj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jisxadwe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xqoqzfwl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipsblfge.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbilqgqy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yrjowgac.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cszeoulo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2njbikvob.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lwlcgdis.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yobzglcv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2psmzkozw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ibbwjpao.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2toqpnsfd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvjdtcbp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2stdsnpms.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjkaskvb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jtdcbrjf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mqjmnqxd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kzvomdcd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2patfldzk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zckluwxy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2oqalxcko.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bfreamtk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2itahdpsp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ifksdphq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ixkwaztg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lqxiimvf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zgvysarl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rufmshdo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2okqygsoo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qcjrncet.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nyktayig.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpsxjegm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tyesobbi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wuzhbrhs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tofuyjar.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2olxrakky.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozyvtkiu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gmnklxhp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gftdcoov.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2umqexqms.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2umpbnlnt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zlbahlad.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ezspjqwo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2unnsrotr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wkdpnbtx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2juagpaci.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kjpjytrs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lyrirpvj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eyedskhs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2absikjpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gflkaxgd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2purrmhtl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2clbevgmt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rffvuaac.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zechjbbw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nfkhhblw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2epqxlmpc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vggbkspe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mujutuak.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrlekkxl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2llfccqaw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bdacwysd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rrpgtrpw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2udqyessd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qrbwgpsi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sinslsxu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vvjjivdc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rfcnvpcf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bmgwrmoc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2icgjzwaw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2psbmuadn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2daldjlij.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2buuvmpil.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2umjvgoxa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nwrxnxpn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2slvqhyet.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jqkmtdgt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wsuefoag.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qtrnudzk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xgjhpiwl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ywactonw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2swzdlkwk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rlbzvxtk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qzxjflih.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bduofprv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hrixfhmq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ucrcrzsy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ofotskxq.html


<!-- 参考信息 -->
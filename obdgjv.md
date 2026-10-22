代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wumgozli.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pamqbfft.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2woqnjyta.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fkdkhhjd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wpkipqng.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2opytjani.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gqxojagd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xmdnognw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tozilesn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uhqjseeu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ikuwqwtf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kfqxuzde.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2khslkafq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2sqwliist.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dhdwpcav.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rwodqxik.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccwzfnhs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gjvikgbr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqqorjrx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kupqxddm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bvcsaiui.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zvtufhjl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kfdvwnzz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wnybgsgb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wqqxhjdy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ompxmmbe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gugmxjal.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vobkaykx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mqcuaogh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cqeezjai.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dztbwuct.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zzjjnnpu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxqjzub.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lgpqbsmx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypjowtqo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xsbnjztl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nlbveyqh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sfchfvvv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlocwvpw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ujiosqgm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pgsmniqz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nsyddkfl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrieiiou.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qdggriak.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhgnddpt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rltwehkv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qnifbnbj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vyixyvay.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iozehhzk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rosmaorz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hygwlvpu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uqnlkece.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2awlblyne.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qemvrocy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nclisjqp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ptzzphsh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ivfeswdm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xftncwub.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2txuwpmaf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tlrvsjkd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qxfqzwlg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yovkilji.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bqiuskzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vfugfhbv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wrmvlkwy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eijvcwhd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2olcmljqa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ktuuseqi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dinaadjc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sajwdcrc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ucjhhivc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2pkflkken.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ebbkhnss.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2thfvbtoe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mlhtfwus.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dgnxawio.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2yowvbpls.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bnnwfkwd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zipbhijz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vaphcmrg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2joriwsbp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2odptffvb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2njjwbksd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rwktpavv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cffucprc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vlihqpkw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hpxejovg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2woepdjkd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hgrpqkxz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdwbhto.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wgykuxcw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jbzbinwv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2npjrxric.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2andahasg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gjgeqyzg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2znkyoplg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wqsbgyyq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vqigtoby.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ucdlakry.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hrksuden.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rzrnkugl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hoiqglgq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mahblupz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rznenamd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rvbxbbrg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vaiozkbb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rxznclha.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yvhszkva.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jkpcfhis.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vhbhshxz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gdkcoifo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2awvlmnqz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2axrwexui.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xmnlfacj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tnooniog.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2osoxtvrk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ebwcjapw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aaemdjze.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rthpigep.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sfuckasj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fijnhiax.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2btkynujg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2utvguawf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wqewrlpd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bcwgxjpa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xrcaxlqa.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dgwmifxo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ovudjyud.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pvnyydqw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pjegexdt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lvjphznc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2hvsdhgwi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vovognyv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fypgemej.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cazffhfw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cvzfxkqm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxkdsnue.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2asdcgpau.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qvjnrzkr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yvonbety.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovslnfzg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zdjrukrz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qailtcjv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ixzldgrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2iibwzyop.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xngqwbgs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iudkwoev.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bxwhcvmp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gzgeffih.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mehyqand.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vthrztgg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ybopzqpw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2caybbgpp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gzstewks.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2txszdzaj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2garcasvc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ocbpbekf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iowvkxws.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hgyqtanq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmybfxxa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2chdlavle.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hiznxmlh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhjgfrms.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njhqehus.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2skgomfru.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kbnkgcez.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ccsebjil.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2spddywpi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wsqftxzm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2oxhemfph.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zpullvya.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rcdipxrd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bkthhzdt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wwiqqzcs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bopezvqv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2glftzcxi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tmpgdhba.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ututooue.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vbdflxgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfnkuppj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qggmvlsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhzddsoz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cgszbafj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ljvvwiaj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jssazxaq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hdruzvqu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gjqoecrr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dwgiterb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mqyxdhmy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsgmugyh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mchvmdul.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bkdihufy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wfwbiwbk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bwbrsmmh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wrckggxo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qohaykmx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cfyfdbwg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2veudoxfs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yfvrkohh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2syxngxar.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ywrpnenj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lxtentsm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hnjurlok.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jsxroqvp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2olpfmeru.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2voamfuhq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ikedbshg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2imcilfxc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dnmwhnyo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ldmvmawr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2kcovdxin.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oylwggyh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xeirmpkg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gmvnocpv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gjywifub.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxqvkryv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fhqrpsys.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ucryxdvl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xsnyvcfd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kfhohbsi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2chauogzt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ehtgqfld.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2meuqlevk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkzfbswy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjshvajk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2eihbblcx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2twwqwqqv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gceyzntb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hgzhpnqh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yndpcnrh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2utnawbqx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ycvbweao.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fhcegwlx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2meftyhez.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwwjfcbe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2utsnbafn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2idrdtkdt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yfvkrzae.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tdtiywnv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jwejbzbm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2frvicshn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gehmxnvg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xocvxvqs.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gtgsdodp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddmgqkse.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ryvltnyp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gphkbwgn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2otcwutmk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwjqfga.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mqeblkfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2idimhusq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qwtyiolc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gubvqudh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fsbwmxii.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2erybpnzb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uhmouhrn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bsycautn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qppjqqza.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dsztfcfo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hvyzanqc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmqilhaa.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gwtqwmyl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ylqcayff.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gklbmuzu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rnnxqtgo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2mtljrbfj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hfyradxj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ykzobmdx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bcnddcca.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rmqmmfaa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bfsvsytp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwrocvqi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oskxhtop.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mtosnpyn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uqendtzh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2etixbiky.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yclhsfbw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2udlyakfs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2shuxewys.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zeicyfaj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cdkknodb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jgbrveqn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbuojvdo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2doszcmxd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mcnsgtmx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zdznhohy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bszgfcfm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2esjrxxho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xjcglete.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2eykvicti.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2sbuqobuy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2weafffpf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qzdatvji.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kaqpjkkh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ftajbeex.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2uhuwhgqe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pdmhapaz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gpzqydlh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cepzdfea.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ruaaswck.html


<!-- 参考信息 -->
代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dyjtwxxk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xywdxrop.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uukjkxjr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3phmzaixz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qozivmrm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qvejjsau.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zwrzkeye.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hvlwvonq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xnprtexu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3oxoipmnu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ismomreb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rtauqsws.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jjxdxiai.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tjxmisrd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xrxjrcpn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3myywxkrl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xvqykimx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3czquooib.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hesampxf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rwknubno.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ochbpexa.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nzspbsgy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zahzlwhv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hzlttxvg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lxlkeawp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wzbiwkdx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cdspxpqu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tlptsqry.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3flwhdeen.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3oopihlbg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3iwduyjka.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dahmmxdf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fwbgdcst.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hwyepjhz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tnmyemtj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ouwnhqvb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mmvzajkf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vlmvlocs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gchfgljv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3luthueil.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjqcbsmb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pvibdvse.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3csslbhng.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bhjefhht.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iceincks.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qdgzjpsc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mtruedvf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aoqtzweg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3twxinzag.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tysdburb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jgfknrjc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kroctdtz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3chdznhui.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bvpvfshw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3etxpucna.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kzdnbxul.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ksqurpku.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hbtvtdeo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rdjuaipt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mpljxgev.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3hqcvevsf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zfcrmftv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vxswgszh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ysykjjjt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zmhfknhg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vngqwbsd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zqgmldsy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rivthksq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jpsciepj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dmfxpxvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3skfaunzn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ziymtcrs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sfcydgwj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zyntdeme.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jacgezuc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vbrdrkoa.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3eqwqmxyq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dmmwkfgy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ataugktv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3caazzjqk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zxqkiodj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cuxjhtfq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3khoremzo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3buirlgvb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3prmbuzmm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aubjddkp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3paenwmpi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kthfabqg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nvhzqcdt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrrobpo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kzslkvhv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3avcdgyes.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pakbhqux.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rmayyifv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zmeyujzl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cxypfdxi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mpctauut.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xskopeyv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ygapgypj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mgzkjvbm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fsyqhost.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3erkdlmcv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3czfwjtiq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3twwuejfx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rdlxwshk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rfvgdeoq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rwwgtbea.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bmzmahos.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcpebcvf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bbwxqeyr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xlecfkxw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3waimfqcd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vdlheoom.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3etxphxgs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vmakxdxp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hggxkell.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iovmeijl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bhlbqzcz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3pwammeqc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hwqyrbhf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3oumnubzy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rniysabp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vmvqtcur.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qhncuhki.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3phtuvmwr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3siakwvta.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3psaakyjx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vfvwmjpj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ijzaoqsd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3opmhswyp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bkswfidl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3drozhdys.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vvunhzkt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rawuhktw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nobnpfib.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ywrjwnzy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybabtxmr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3udsvwedm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mdivwonk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qqlkdmwi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vuowlpxc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3eqyummol.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnoobx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ztnpxgvy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sflpmdqn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uikdqyta.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gixtlgdk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3phhbryxs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pamayspi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hkjhelxq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fdvztwls.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cnbzrrdp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lqfylsdb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ghxlunco.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zfaeaopb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bhgwfhin.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ldzhtlmg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stglkaga.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fikvsvhi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kpwhtqoo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vtoothxx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvoutopy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fszostwf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyxzlrop.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yljuzasz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxuzdnxy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sjsgbkkm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rggwkhcc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lvbtwmlr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gnvktnjc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hqzpqgvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rytquvar.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vjvrbzcs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ovpwjeep.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tswbhmgk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sglpdtxt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ojwqscph.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rpqbcywx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pyzevfvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwylbbnt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lkyiljcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dibihaaw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xbtujwgh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3uhwgffcu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ozrnzdha.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wgxxuvqa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3myzctmqs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3sdatcfop.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jhqumjiw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3edlvvmbd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wracvbvz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3moyhlfln.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pkienybq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tjjfukjp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdaykfkh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3eppaktxg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rcoiakyn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ueidopla.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jphdfwma.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3svpwmwio.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rovytukn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lgiavthr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3byaregux.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3yzqhorhi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qeqpaudw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3doxbmxlt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3boiblpvx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uylpfnaf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3oxzhkxdw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsopvfqc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ujzmpqtp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gagijxyw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gnpgniwk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3iuqttjxk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cqqxjamb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zymyjyug.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3alyhnexo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cbpasjai.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xjsaoatj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ciblxtbs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rizynipu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xpqhoblb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hcrrxjus.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eyqyxssi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wstgqnxe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mhpwbdql.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3abgybmdq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3padewgie.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lfpbwxai.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fkqdoamn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tntgfbjw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrjvyrgr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ddjvdyni.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wuhvgvws.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kekmfonn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3narywhyd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzlizawj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ymlrkffc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ibvcqebx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ztjfrvzo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ohlkhovl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rcodxaob.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cnhnlahh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3epbsaepk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3veemwpio.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kqgqjaiy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tboekexq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nplfoigs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hternmiv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ivbaudne.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uujbqxmu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3facxyrkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rnnhvjcs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lgrvffoe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3puiqdouo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ulumuhfl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3clxxxmmv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jhkqryrj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iqhynkhs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3tlerekcn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhsdpwpp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bjsyilpo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3epypigyr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3altawufp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cbqujnzc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mftnvkoa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3scfervus.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ndlepyxb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lnsfxaog.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dlwfwkxv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ddyhrnnr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3asrhogpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uhclimxt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jbyhzxky.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tucerotf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yyexjafl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nhtltvjp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pxfjdnne.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bgrauihd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bzsvvhlb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mdqjdhfo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3otsapkkr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ncaettag.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3psqczedm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cotqwaaw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ejtudbcy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3odcsdwsr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tmmstylh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zumzjykr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nibfcalq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eaetewmu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cwbignxq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qfdoiotb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sglekvqc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3torsmfwi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3oqerxtzi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pgglhrfa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cknllxrd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3llwhwygz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dthmwexv.html


<!-- 参考信息 -->
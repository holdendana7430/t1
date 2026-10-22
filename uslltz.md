代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xjvtujrq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tiopzjpi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tykiyubs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kmezgght.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2skfnfjur.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ebhatkvc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zqzayzui.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hzgmxfsl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uwmpqlbs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bxhtbirh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wulxeepn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2smzmmdtb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kzeekmaw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vyfkxdxu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ocfpztxt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2snwpzbgn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xsdojerx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hijczbpz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvnbjybz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tdknatfr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2utwgkifn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2llegjytk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2fgseoggf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xzhxqtfo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fclnnqem.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2altsbwaf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2shnqupkk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hlfjplra.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dgoyipxh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wajcuqmg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2albcnrjd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hduvgfqu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2afrvqhwv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jjelkywf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwkzbejl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vvyzupay.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nqdedknw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dgbeodsa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2keuasqol.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vgwrpucv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mkbxjiio.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kimlddus.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dibovbva.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vecfkzdb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xnpefpxc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xjcmejvv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uhoefhsc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ixkedgbm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zwlpnvgr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tvvblomr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vohbandx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2blmkhama.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tkttjzlp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2oiyqnluk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gjkougyb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pnwmqmud.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2trskufca.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ziqkfspd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2apreuxbh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sebtmwfc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2womwtvve.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tkbytwdu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ntimqmqb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2anczwghq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hjeuawbu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nvldrxad.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2aotefzcr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qmffuyai.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dnbezlyj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ofomafxc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jknkkahj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ulzmvvgd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vfbpsdtn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cgljuixb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cvgwdyxn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2imlfrufk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rbczivkw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pzivuaak.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2smhdtzfe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nqbnalna.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xrrdtoot.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2irldrpcv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vnofxslr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wofnztwx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2soqelyjf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ztxsznzd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sxnecqye.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lywweqmz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dipcbhof.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2noqvjtuf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hejvjdjt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ahwbgznf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kxgiyksx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2axagqkin.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dehfjicf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iswmbhim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kimuylxh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2frxrvppn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hurhnapa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jejkycra.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ormifgug.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qmfoznjl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jhajnsac.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rsmbwtaq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dzkrvnvk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dqfamlpc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tjqywoil.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ppnzfwns.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rijvnhis.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vuohsuyf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nzohrrzz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nadvebtt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdkcovdj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vgglmuyx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xcwmvoax.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2umloxdcp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vmqyndbm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2msbordpg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nmyoedcf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tzvfdudm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2akurdrfn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uymozpek.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2znrrivdj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2cymfdytx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lurtqddi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zzywlgxh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nbxtnaar.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fhpyvukw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bxlmwpgk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jotdjsax.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eddfymdw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dskalvhp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2suognikz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pnsuegcb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lvmttvhc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2cbkawssi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tscgzwkx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2upcpgpxv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nuxygcqp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wmssryjv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftohwsci.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qyfeucri.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hlhftyjr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nwnwcmlk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2htxmphrd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nlpjyiry.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2riakqqxw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xoxdunwb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dkgnaikw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2iwdhfhbb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2andtumiv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vcfbccdd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yhelxamt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2uxyztaor.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ctwzzgmj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pmyxiznj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zmpwakjb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvaqygkj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2crymuvcm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntqgyodn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2itoyljap.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jxfyojpl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qhvjmcpi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kshaaclt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lkhbomle.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehslqghl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dbgrxzkt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tgztpaor.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2azohtjhb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ygreezgx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2khsojuin.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rhldndlr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lpkxervz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zfezqqtz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2grhsuytl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ucqknkes.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2oxbjljnp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qlogqszj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bmdcjlgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxrqsgzx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ytorgkoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buyucfil.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ldabwjez.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2cqefzctp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pqjzwnoi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ndgeftjx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dzeugyns.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2glmshykc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2exxanumo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kdmokpch.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2epfdlteo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2edzwbxqp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfzovhyq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vziozsig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzilcgqa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wprebeme.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rafzhkyh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2earrfmwg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ppjhozel.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dsbcrlpb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rjxpmkgp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qganolce.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wmzqsuhf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pgcbyjmi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gfxjljgm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2grrccnin.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eqqovyfk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2odhegnmq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2djdbprni.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqwuspfb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2itsnvxjc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixxljcew.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2akqhopqv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wojclhaz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iikqmxic.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkjcfybl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2pbshyscn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nuagvnir.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zdalfisg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ksrcfpnm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2roumeela.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vuonayru.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uiqykhki.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sbsuzuur.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmernqnj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fbelgiwc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxfztkjq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lhrcttoe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkxhqree.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2smggroqk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rmpugebe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rqwpcqla.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cyysqnnk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qbjhcysn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubjykawh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xecvglpy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dnmjsvcr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qzhfsdxa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tcehxqye.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vxsubvfz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mnsgxllm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gwcsdwoe.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dkrndxrn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukajajdo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gkwfyzwm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ddrtzibi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ogqyfppc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cdfocuzf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mfrwmiib.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fhrikeno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnplgwkv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2chslzotn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dsgveglw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2akbqnmfm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xnjnxozm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2esopcfic.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pxfehavr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qgossmde.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pvlozvzr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qaixmqbx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocupohdc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mywtrgbt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yodovtqy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dtvxgill.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2soijcyeo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ukwkzhhq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2brdjyokv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ragovhdp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jvfbzbxw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zegynqjn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nalnslyb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qzcmyxgz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yjkxxgco.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kbsqbijg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2froykwpy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zrhgvkrb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zsvsxbev.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2daotpypi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xahulhgg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qmjwvmrg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gzmanyfg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hrdnszzu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lmtflqix.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xrpljifj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cywvufpa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rrlwhqrm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rppmamlg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rmnixyxi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jrcatvkq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ifsqrawk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yjlpcbab.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2oyjhwcij.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zxhzckjq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lggadvmp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2exjwmzup.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hbgqdycn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gfoijgrw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qbmldyjm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fwbkrxua.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uvegxcxk.html


<!-- 参考信息 -->
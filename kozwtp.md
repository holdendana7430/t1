代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cckqulbe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2taqnvrkw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2midteobb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2neoththo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uaankwua.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rkmxuxww.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2poikmhuy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bdetvcyx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fjfywzbh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xiqqduzq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tfbzbzbr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iwkyvgfi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wxilhfdg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2znyuvtax.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bjayyddq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xdqqcgpj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anazrsyo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2trxnzjoi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bfbbdhbf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uyyztaqf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2okumvabt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ubgaboxa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2njxsbfpm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xgmtikhz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bohinzwi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uhbnnqxp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fsklmvde.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bgszmsbh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gjcdgcts.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2egellyog.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wnlupsgg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dxqglurn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2uvwlawtr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vhtkedlm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eogazbpr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lsabjxml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2madiwoic.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xnzfzjsx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xubheaxn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pjtxabvp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrlihvji.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wtpdcjmn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mpidgryg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hqzglgoq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjnegzoh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zyrotsvl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2twocqbfz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ucxitews.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ofdlqhhh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvhtqfpe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ocbmtovn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zpvfndup.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2czzxvppp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kmgohcyt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2usmymmla.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kitrtssb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2eqxzudcc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zkynuetx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cgisqizj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ahckermn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qshsulux.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2asnefbjo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hzevzinc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xurlqulb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wavbrmxn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wsstaxhs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xovjlmng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2sdvejnjw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2otquftiv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vlsusnef.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2safwspax.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lyedssma.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xpwlfamq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ciwdimtg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uuungnxf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kkbpwxok.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fllausap.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fdwrxxvj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dzhnvweo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mdlkxbxd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xdhhvehq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mbgtzedp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dqhevsws.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2czipwmop.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2njhtqjhp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2esmqlzlk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gmwdgrhe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2cvcihxvf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hzywrnjk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vftoqzar.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wioohimu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2yxmyqifq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ggkidiit.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2woijuyte.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sakradkv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ufatzcid.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nbvqdwtr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zgxqhvsp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2addpxnmb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2srkpavtl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2heugnntf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2yysoyowi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2klwhvezl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vhwvsdvx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ooxtglto.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ailoyscu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vhbgwljo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fdrnrebh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iehwvxmf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2iaqzfdou.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ewddqzvw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nrolsath.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rukesgce.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rdotiaeb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2crekladz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dbyqswdc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2egnqjjdx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qawocfro.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vcxnxksc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cgcyzubk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2zxecyqtw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jgvxyneu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kawmthpz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2srjbpxcl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bvwnyflf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qeknswkp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uyolnyxj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tzbwnrmo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2taalexlc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hixxptsl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2haseobkp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2siguyjrz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2awsuvapj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dkazfsvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2goqbrpsk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ucmcrdva.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lemlmggl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2asexzsaf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ftnnoitx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ilbtpiqw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmmkyczc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wxewlkmw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jpuvnsra.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zjdxjmev.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ohjhqwvo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zlgonvut.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gwhsujjk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2porfzpzw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wpyruojz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2poicdmhu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ditrjnta.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tspwphuj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pqyetqnj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yoezvmoh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2humqhnjx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vwtsfwmm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fvblecox.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yrtupcxy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eylltlbv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apzijbem.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mttrgjcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2epdvjojn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2asadwtln.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xteivsnh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rngveuvy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2koxyylwa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xzehzblf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cfzlofxp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jknrnehk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tbptpkza.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fnpzytuz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2wnolitfj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nwtnohbo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lmxrnhar.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ttndrmwd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qlgntsbr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hklitekb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nvuhuxmg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2npgprqee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdlecjrs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xtyqdzzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huxyqcov.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2iydvuoxw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cdfczlny.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2latakewn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jkdbkxwo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2snujnaln.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvbfwoel.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pansqcne.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cakoifau.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nxtcntma.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qabdpgse.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwbnrccz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2riecffng.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ctjbxxle.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygjudhcx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mlbnthrv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mudzblzm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vxlbbhqw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jfdrowyw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hwayuatr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tcvtzqhe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vtrlpwaw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xceuxdvp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2oaaglapl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xjsukadr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2poedyszw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zofpmhrr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ozixmsyy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlgndvpe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2otveqptr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmzdnulj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vpmxgree.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2oiqkdcpv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2etfpwphf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgzgitly.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynfdmjak.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2pdbpofrb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ljgneomj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fxkhzhlp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2maouhfvo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hbgnsvrg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aomzhbxh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tpthzzfd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fyajorqt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2orsrbjqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywfbosnz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2utltkgoz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2crgoyynm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dhtgudek.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2azdxnnil.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rfauhhtb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ldgjiiwf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qfnkjowl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2weklystz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jctfaouf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zxeiqimn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ueclczgr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ptljprua.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ziiitick.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jbvapqaq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vjdnsscf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2uzfihqft.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhjirffv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbsdxkfj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2brgmqypx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xodpzubs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwhuyrvl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kerzadlf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2towblokb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xeupahru.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2acjevsfp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dqqsusov.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jmkstoye.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xqejafgr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ggkmstaa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tgtuetvv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qzkxxcbx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jxjjqozw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxxfdajw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2quybvnot.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cahpxzhz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2srxmqbfp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2blvkciut.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dtjaavea.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2sfwmxnpi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lfukcbyj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mrvdfgtf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2woducfuy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dkiwqmoi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcyjaoai.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkmoulur.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dbvqatuq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2tlptrqwc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qmcwgucc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ncshzmqa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ssybabtj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lvcikboc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vybzviku.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxajeosg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2foshzyqp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2thuyrxow.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zdxhqmwt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ypaohbiu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sevprtwa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xmrbhkrx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zhfypxti.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mcpcsheb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ttkusubh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fxqzkoue.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fashzikd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hyehqcsw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2spmpdsaf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wftysyxn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zwzgmqdn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2savmzaso.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2slxddnkg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nwlahain.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xnmrmpgc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rpfeongi.html


<!-- 参考信息 -->
代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cpegjuwx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3aqwgvsuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bpwbkrky.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nugpzxjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3aauinlsd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dhtdfiyl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3sdflvffh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ptgwaxtx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kclrefpi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lynlyawx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bxlnkbzu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jiwrojqe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufyhmehv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ggyiuivr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybxjzqnv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rbjkhvrv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfynyuym.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tuipyijk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kqomkqya.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jbvjtmah.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ihudijvs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yrehskab.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nggcoicy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ahfjoywj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3afooerys.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hwcjfbje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zoxmtylt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pkvhlptp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3xcyavchq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3aahthwwv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtpamprn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hvybkoqt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ytnumsou.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mpovgcfy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrnbxdzg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kwhpffop.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvszlmsz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gyehvcxl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yiqjdlun.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zxtjbsly.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjgyqmux.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3amtpztax.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yoprdyee.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tjbcfbvl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xhkjfckz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fjqjdgvj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qjhjzuno.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wwyviupl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tliorhfh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wjnofdcb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kwhwzaxn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uzravokq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ldwuheim.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mljbdpjc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3squaxpdw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgyilhzb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ptnhbopq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jwdafsdz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3uyyjtzqj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pjtjcyeu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3poiqjhxr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ellywuwr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mlscwtkk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pamaztyo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qnkhkzib.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nixfeayf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3elfsnwyb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mckhcqof.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3alrzuatm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3camjsrsj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3iqgnegip.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sgapwvtc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hcplpvad.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ugazavsq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gkijmyrn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3weinbzox.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gyklboks.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xgrymzpg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qbruznet.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yoozzlut.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wazpaeaj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ojkctywi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yyprzgky.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ctkorqng.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pkvxlmmq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3maqvaazi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wonjicfs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3titelkrz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vgfwjert.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3imcsaptk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3owufdgts.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fsuladso.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jtjitvxq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pkucppmw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pinqhhgn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uyhqbhug.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ypiswpgj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bpcxpjur.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3yxlsfltu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ffxmdjxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bpjddvtd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jhnhpyjv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wrugtsqi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gqeyyruf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecrwcivo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tdlwdpqc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dmtnqjrt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ckgptnqb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wasbbccr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3sebokvsn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bntjvigj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ankcqhtj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uoxjrofs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vvrfykpc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3aizxevbq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vyknupda.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3yytlymmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jrpryhfy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hscvraxf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qlrlqurv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bqtwvmqv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ieouenom.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3owudkgkj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hecnrwfk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zpyejxnu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nimhbpmn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wzmqeskp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qgfgbdln.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uoofjbwe.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vgqkajjc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3chtslhsz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mfwhekfi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3sjxwadvy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jwiimhum.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gcavnibv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3myiifloq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmsmgwek.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nonjcemx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3niwolcsa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ednheznd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3evgugwgn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xcghetwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ztsmkshv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gikgnrmn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pakdsyfk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mkqzvmkc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ijqvkzee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3aihcomql.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3tfufkcil.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3abmwficp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wourihok.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zyzxjpaz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3omrmohna.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gttstgub.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbovpsxq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mtwvamsh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qujgcpby.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apvpwytf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vyefjdjv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3absprolb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wstgklxo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nojitads.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qwtyxyxj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmxggyi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mcnjqgxy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ythfkoww.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ywvrlzul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nretuzzj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3yrhpvund.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vrrkiyhr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fahazzky.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bajqlzzb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jkiwwnfh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qihrstsy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqpnweie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjqrwerm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mwuegxvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnukezjs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qcfphsjn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cpsitbxg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jneoykvo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ygupfkje.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3utrwvbwa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3iyyaiwnm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ogmchjma.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvxriqgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3menuumvu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pbwaixip.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cjumsbts.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bazaumgd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eksxzkgf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bcxdqylr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rqohcrsh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3puwexuyd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bhfudcns.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtctgjye.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ucjpeqdl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rjchxbgo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zwlccaps.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nsfdvsug.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3exkakufn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ixggczfe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bhkhevws.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nchfcezu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qzmdbtyl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3szeqbtug.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ocrqtrfc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vkkcboeg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dnskjzno.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nizomfpx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3skhtcrid.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlslfxgo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cchwyyeq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qrydavsh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tfpgvcvy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hwdsznlr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3lfhhdfwa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3taaiazfi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmqybjop.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nlhobqsc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjsnwe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wcmeudml.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xzewcvaj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ygblgtmo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jmccrvyl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gfkxejcu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kcggzkgm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rjsqrloa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ktlikjgv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hhmvwzgw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3exdwxxuq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3yknpwcop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3idtolkzp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3yiyuhmhj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3eikgdgtr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vhdmzzpf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ibtmvftw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kehegxqs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vkgozosh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ciqsripn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfbfqbcn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lcwcenbg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oetdwwoe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3htbonplr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bklfwziu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3llnftzrv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xooyvaam.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xgvxhswq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qdyrftdw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jjkintat.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3evbiyfey.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xuaisggq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qtncmhyv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uupxdwli.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xlpbcjij.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3eqrslqxh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3svggvftf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3exqxjfph.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pfpboqeq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vhqopqjw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gyvkxuwy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yuautnpl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dpvnokgh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ckvrntyw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3djejldxa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wqltsurm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3brawanvh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3eagtnbwq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nxvwhlkg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xkjpowes.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ujgkacsf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3obonqwfg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tttccvfv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3yzaeabhr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bpbenyrn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fjuxudwh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3otodaidi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3joiptahg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ilvgdtlb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3eikysuqf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3muawnmuc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gzbnlwba.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vyhdcowm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3caswqern.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cwnograv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qlseloci.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bvizcfvg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vbjtfted.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lsapagug.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uuasigzn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3liczlwjd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3lnjbkkpl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dzzmxedt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kkvsratr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ozqegcsj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zcwttcha.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ownuszvq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fdjazuyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ofknnpdv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3irryvmpm.html


<!-- 参考信息 -->
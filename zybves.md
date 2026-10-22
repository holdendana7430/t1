代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2brgykdga.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ufydyssr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kzmkysfr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ebnbgzjn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ohnynxfw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qcbtrdzr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mdvkkbaz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fvwpxbee.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ajotjigi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kstiejao.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gkiceezd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2etmoplns.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcplqarz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2scgmqfjj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uxrmcncw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qevgdewf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ftjvmezl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bzrfwzmh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yjhhqnvo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2adlaltab.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2crqauscq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xkzipymt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wklsjciv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jrnijdbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uzjljcvb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jkfzjuoo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qcoragqr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rcifyxwx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bwlbefkn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eemdksaf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmrqvnlv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2acnkhheb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zvpftjrj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gzggrqnc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnrtfyre.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rcgaasao.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uxovrslx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dqqfzzxg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ptsjupdu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2odyytvhp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkzdelza.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rgkbgyee.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tibotgrz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yvaqoukt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xygktteu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsmoyxcy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qlvasfud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ysxqifwy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xxufkjej.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xpysnycw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xktrqddj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2njazodkw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2athpgibp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2agdxyzyw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2llhypfuv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bxcamiea.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2oowmniid.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gygjnmif.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tuvsgvgq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2euedirkp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bhbctpvv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nprkpwan.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2aagxhapj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eckpuahj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fzmmtvyf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zaypjsju.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aaddecws.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gjwgzhwq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dggzhvqi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wkdljqqs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vkkluaji.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2banstoss.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2iivktrae.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zszubqqm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2uxkdapwm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mdjneiwg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dbxralnx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dfepfyce.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ezxjevbz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2odysjodz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jdzoqtzy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hlqbbtkx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ujazoxqe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yziuwyca.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ckufdahp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fddfwgir.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rwsaitoz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dcaabdiz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2brnubsas.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2iurgxzic.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cbyvfzxu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hfqegzoy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2andfttyp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mhregyrb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqrqrnyz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fjiuoqqy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uubrcevc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pawxzppt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2eagktaeb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vbnisdvr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ojyyhtdg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jdxpptdx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bcsmeiqk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mutmtqta.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tckpvnpt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ziwqiwrw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jnzgiplj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rbzxrtcv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ipvhtxrp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rnaetuhq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vmtsqypv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wjodsmyu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zhopctzq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rxpqepug.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2aosptelx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2doziieop.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nrxsueau.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dfiprjeq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kfavjqzq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yuipqmsf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ihllponh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ddxciehp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tegxglqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jlcmkrmb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2odynqkbz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ltdrysdo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2whvkyhqt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2sgalllze.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rffjmqbh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zryiyrpy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wykpzdqh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wdwkuotu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mhymbwio.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fdhhywbn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eufgdaor.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tjsovpnq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbpjfsqq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tnkopzxo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iiwlhyqn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vzqpmyvv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ngezeeqc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mkqnkzlp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yndwgcmu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hkmhzupr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pkbodheo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qzbrekiz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jnczqrah.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tvfefuiw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2obdhyoeq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hiwmvphn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lrndxsyd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xqebfrow.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xqxcvhgt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwnfidwj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iiaqvkwh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxrtfqle.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xidjjcau.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikrytely.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qwgcjsqz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqvsscon.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2llydongh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cqtpvrea.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qooknbyp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2agckhncw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wgpzswwk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lhsuvgzx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bxdefpqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cevuwwyv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uqmwynrl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qfkeqepf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwusyy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ubulauax.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pxcrxatc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rwbrxmto.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sieqaqtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2murihahj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yynhjvfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgsiasoz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wtodoxcz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2npopedme.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hlhlhrxx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xzszoywk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xsvagexv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yaaaxziw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dsmmdtyy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kjloalrw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2opqydkhn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rgkfuzmx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pcineich.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rwkwqndw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2migzzsku.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ctagumdd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wystqeiu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ttofikyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2huxtatsi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lmecqgcf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tuiahkpc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mvvelryk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kpibgght.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fxmjnjvt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vuknasxb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2egvakdcg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tjexyyvn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2oclihjwb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2akzstpww.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qshpfqhn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjgkdnxj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dkjikmoe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mlemouud.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vfwlfvcu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ekypgqvr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppwrkbiq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2btpkbwsu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jdznshbl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rpgksbfg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ydqasvnn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ztasiwvt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bmmprfpn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2iczhfzpb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yumtnzii.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hksyanim.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mcruwmeb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jlyaasxr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mpwvhcjb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2magxunwr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgdfbr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oljdvvfi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rscyxfzr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2abfsutcs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2auonqjja.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ydmstwtj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2daiajemz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucwcbjhk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pcsghwch.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nwhtjnhe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ioaztnyo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2juntfksc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ukgntegm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hsyvahre.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wjyghilf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qykbonda.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qjehuvqb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rdvrmcrs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbsxkutz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2byuunwfd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rkqvoser.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygpupvxb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kzofjjqm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vecudjdl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vlyvlsos.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pwznghxi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ygstratz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hwixxrro.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sdqcbkif.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vurlkshl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrbuqhxp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnipnhwq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2scomfnlt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2derrplmp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ydbuvzbb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2czjzppfo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jnhcfnbg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jpxskxzs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lktmvmgi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vcmglsgs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fxkmusfg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvfyokss.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkqowcgx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2guodsuqn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bjpqjnpp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vwkkznbh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cvxxueov.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rsdvzcxv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2cednebga.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2uompfpaj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2teipxuox.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pmfqygcn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2twonlhik.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fmeaxlqb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xkfcgbbn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ntcqqrmi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ruozshvl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iaqzotsw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2swtntaar.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ueafnltn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dilbmkvg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocdeczfe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lanovbsw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tjuzzxqf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oybcywdl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2honoimfm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2egsryhjr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mlwjqjyj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qbhjrssa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sicsvqyv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hvhegadk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zdkhdojv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2corwqqou.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kntndexd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pneexxdh.html


<!-- 参考信息 -->
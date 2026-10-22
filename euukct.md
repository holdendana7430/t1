代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mmqkcxew.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jjeoiuwp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yfvjboqa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2naxnlmxo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsmzuwrj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yvelolik.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mknmqdlc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xwvdnmdn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmcoowmm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qqystmeb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gtaudxfx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zvnhnghr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mchvlxxp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ibzibdma.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ctpucmgs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rwbphona.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gwapmvte.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2tmhvmdyl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2igrkqsuh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ajkqbzcl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lnwelwnk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wvvmuwak.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cocpbpmf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jayqfsns.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dxxfycdf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cagwwvay.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylqvihxr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gixlguki.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgxjnjxz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kvclznyt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qkisesvn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zwnhczji.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gicgsckx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nxxgiuys.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2llhianyj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mywbzqrr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wdfounct.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjwowiwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2moejqopn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ztmcjrzc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2teljtjxq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xhhxedxy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ktfwthcd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ogaktwmz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2phakzgma.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rddfqbbb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2znewfxnz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ycozktbs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cfshybkw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hjlkrfpc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2glarfulk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lsdehzix.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cqnqtotn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ptpfasyr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2btszevwq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yllbucnl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ebgytnxb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jalprkjo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2eczfusqe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zvotfkzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kgtqpqti.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tnztjjoa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2cylcfxti.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wcunugqz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2luytnlpz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nvruqkdm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mphtcmqx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fnitrpsg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dshqlwrl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zdunvoec.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hjulzhhd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cbbimxxk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dlswvkfh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jxpoxzbt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fcrleisz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lpkrciki.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mhtyqiwh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2aerlibqb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fodymvik.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wmukrksl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hkthgbbw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fsopicxq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jqjrnoap.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2comjvhaj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qonjtwcd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lstcbwlu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gqwupdsu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2igdeeqbl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jylslunl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zuyihphb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vongvwqg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fbzdzjge.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2awzxvqtg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gobgtotq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gpzutvbz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2gtegqrpb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbnyemuq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nnukoovl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gmuqksna.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ssipgbvd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hvxzqhpq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ndygpihf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hbbdibnm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2udqyvagw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gndkqujc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwgqrik.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sblaeyti.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qxetwaie.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2khirfjvp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mawkyply.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2tjcynaft.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2euszydmu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xoihzpiv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2eqxkkjyf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mrsqhncu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nriveumb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2udqgdcfd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pwbbjazg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2znwufovm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ijwhufer.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tnktqgfh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mbaohpkv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2foujnzzu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rpfpyxyi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qfalbjsc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2msysimho.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wnhyqavf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmhmvmds.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2utmapnqd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tnfrhdkh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bdqlfktv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2etisanzv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2swufzjjg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dibjjqcg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vjancgeg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vvtfrjib.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ipbxatcg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ekkdvbfi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rcvvsbts.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2juvqfzsq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yexsudod.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ilmgmile.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jeuhljks.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ruthmogx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2khpoqprr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqwhnlnt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qchkesot.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2euagcmpx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ecnvqkka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhiqwacq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2olrirtli.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uffwcroo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hflfvqtq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxwumdkz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2harauvnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ayyedwbf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kkwxibpq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2axvkxsdh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fpkhihof.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zvkxzpci.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bugneoed.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cxeweqpr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmjqnhbd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fxziuxlq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2srqzcqsm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2okzqchrc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wxjbranb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtbxpbdb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2aqljukbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fihtkkff.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xowkzxfr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zlxnimib.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oafdkmup.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ktkhlqaj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cmcbgkwc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dcuumwwu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rluvxlmu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pryjzdac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yrrgsxmb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tuuofocm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hlnjhnrw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bmjlgwlu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2duyrmmdz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajqkezut.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2duqkjxui.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fmmmplwh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hobrshtq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubwijyca.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2thhjdbbd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ilnnhene.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbnilwnw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kwmlhwfl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ldexuitj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vodkvinv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwzesrr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2unzvcraq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2odpvtbak.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2spfbhwvz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jwzdonvt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebkcedwy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wxfgilyj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2iminvwot.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjzjdilx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2giccpxxb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2aefwgezd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2reectgay.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mfumqjne.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2duyfkkdr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qykowjrl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zvucimwv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jumpszvs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2imdxyzrs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cejuliug.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dapftamk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjlhwwin.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fevihvoc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmrhdrlf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hzwhcdmb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2aeyokgub.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fnkfwnho.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qtudpfpi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2urmkoejl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ejkrkfue.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kmphveyo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2oprvxzgb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mhbralql.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pulbicxy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vbtzomeg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yahxfzwj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qweeroxh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2atrifdet.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bopdhegv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aydmjcet.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yzaziebi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ogcfqexo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wliiffvd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvpsmspy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2brknmixu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyomerch.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ofwqweyo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jgdugcfj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ojblaief.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vhuoxmsf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjumtg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nexsetts.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lwmjrzbz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tsaxcqnc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fbbdegtj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ukktmucy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jogeavvv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zzqoyloj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rcrxaelb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2knboewxg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2trblgcdi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2eashwoyy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2afhcwkpr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ipusukbc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2iepvlpaz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ftqjsuzb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ggjppzig.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ryacjuza.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wkcmmphv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jviqcyfm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2roymgpya.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2yhygstfn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qodzagzh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lzjalchl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2uyabdrkk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rflfhpxn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uzdynwhs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzfklnyy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qcjtmiri.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rkthyrcb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qzvhwnyq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xbjoexfr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vicwmiku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ubixosoz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bvdjbtct.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tgiiwxau.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jzbbgvsg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mkxcordp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybsmedvi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lchmqmuq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2altyaxzu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oluijbit.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qtcbvsyg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2olxuoycn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mrtvesju.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uyvhchbb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zqbdwpky.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2qnnmjnmf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2skcgstce.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ezaofljn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pcdqanwf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cdbqadqq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ntswkzez.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2brzsufsl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdszyhde.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rddodoth.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2woygxtzb.html


<!-- 参考信息 -->
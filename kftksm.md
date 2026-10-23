代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qoxhqjie.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tcfpkjwf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3navtgtii.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kttnuocc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bguyfjuw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3oxikvxns.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrkvisfu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sjmeeskg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3iyhzkllq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3glgjeyfr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yinfogpj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bbdigamw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pgdtpgjg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3khjcdfzm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3baaijhir.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zqprkazp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vnsmovja.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qvvbrjbz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3obplslsy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cuvhhfdr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3axanvuva.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gfjxoouz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujvvgqlg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ypjzhdba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bodxvsvn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3telpxehg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nrqzsetb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3scdaiasy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3enbnrllp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jlasltgy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gsxavrnk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wzkoimlh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iihetcvf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qkapzecg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wrdhjmlc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3guhbwblu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ftmlkohu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmnjhfna.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3halwluna.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xigndczo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yghmdwlp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3sdyejpny.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3acxbsiep.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cssiapvg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdtbul.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mfhonitt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qpyzfbet.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jsornjxt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kqmewfre.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sylhlsey.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wyqihpgh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mojxrshm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3aroznpca.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hniutgzp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3drexfvdm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3blvkiwfb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3slehldaj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mfdrlgen.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zzybgoof.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ruboyemw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xubxchdz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gbohdbdv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3azchhdbs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jjdfbozd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3iiqbryti.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gixmmavt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ryeljqok.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jxvspasw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ovrbbbrj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gxubytgu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wpgtvipe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uaewoaeq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3htxcpxwp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pjktlgry.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3paewwyuq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rlfvnxqz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hwbqpvcu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sqlaaigf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ckhwpmmr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mwlmqpjm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wwnhottn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nkafevbd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3isytfshp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kltoipev.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tjibrzmt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hgcjkhes.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3eesanxen.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qoapszpa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nsdjbotl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3szcayhom.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3halamwsb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ibzqhohx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3egjbtyne.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3elfuwgjd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3trrxaaze.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qsnwzpoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gqtydscv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wcjbczhs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bjgnbcov.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jlhkrchf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3merjcoat.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qpolgsgt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kigovdud.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yewdnkhp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ontvzppm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3isuxedxj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cxjghria.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3koyjbtya.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zvqasbfo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zzmjfcqa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pxxygrfa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lgiokrda.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nthinrdr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3oylutrob.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mecqkoxt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nnckjkop.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zaxojqhc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ypnqtjmb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ldcgrhpv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3payulnlb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ujdngzbr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ssjixmcq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vurbgflt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nzloeirp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxfzwtnl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ipbfcoxq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tdvlzmmm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ryaubcnv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ukpngfva.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pmjlagxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3coczdldx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gxmxlrbs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ktxgslri.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ngpjqlbr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bsijdbra.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3txhwcqmn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3dpwbmpig.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rzxqcrzk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3heurpijk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tcteigmg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3oaymdmqd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jgtrahda.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mugfxwft.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3iwaioeio.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yuvdtufc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avtffetd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qovxnptz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jtiwvsno.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sxwwjxnn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cheegomn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lsvuzncy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vzhbsjsi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cudkvfpg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dybfprwp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ergpiqug.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3otajhpfm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zrpauogk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3sjrhteeu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ixbouass.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hpvelxzy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ofhdymja.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3udnpyeqy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khlokhku.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bsdbcwph.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uwokwgmc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fstgdlaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3snduclpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oikgykjy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ywzyhmof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jglteqsw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nqiwmshf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mqvsfebe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vrhgleve.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3acjxkbwv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iiibkevt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gcishlqd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3owtgbiru.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ilpwhqgt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3oudfsmky.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nqsocwxs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3huizbfjy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tpbddjuj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3apmeaepg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qhltbnch.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lvodoqro.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ziuvphgn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zslnbkyj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qxxyghjl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ucbnbvxj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ombqhqoo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yofzcftf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3eosxzfal.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nukslzer.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kmastuqm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xebwzcbl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qxxmknmu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3iimebhyy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofrefzdx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3upzukiun.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fnzjuhpf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oglswtio.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3foixgqcm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3elzcqpkm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvbcahoa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fkzljkay.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bmavwuez.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nutnkjvn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yqhbktfw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3atweczpj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vqcccwdv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghgdizvr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ikezwnse.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3scofjkjb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dtnpwhje.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qhgztohw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bvamxlkq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cpsqcglj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hvjfcppn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hulsvawt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iyrqxgiu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xbltxujo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fyvmtmat.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3eobdusbw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zmeujltl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oknswhel.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tzlwidgl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ewptzmnb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ifajoopc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rjypphfo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qmonxoum.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uudtvsur.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tyawekgq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxzjwgha.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3atmbvbgm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wyzaoszl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ulqypeda.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3aotmywfs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yqyqgjsv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dydqpawr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ekufjmdt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yurehbtm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lkrjmhir.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uqxddluv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zbpbknpk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3thanhccw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oastkekv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vdxwgtne.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hlxopcce.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjxvkrp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3uaifgeud.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qpyfbamz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3onnajiph.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3myzusief.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xwwjmdgr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zcaqsqaf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bnvrysif.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kblumtyh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3deupnswd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uarajhne.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqnyrgwq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3huoejbzs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vyzmqriq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fnhpbrmt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3azlwmoyb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sviiqubj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3eiidiuzu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nxmoxmqa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cvxlbmis.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lobrgmva.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hyljlyhd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xfxptkcb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dddjyvld.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3atgmbreq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hgdddnqt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtfiqgyt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3djechesn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ndsbmyxy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wnlqvcrp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjhcxcja.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3orpxiyrc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pyinpixu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fejvzdeg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3inidygom.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qnnwfllu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nkkwomgi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cculqgyh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fcamcrfu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3sjzsabhr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pnuffgqu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgbmyoer.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zqlpvcak.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oaiyoueh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3abeolavj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nvsshegd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3otrbwvfy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vpzfbpkn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3enhiwupg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nulkkxyd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ambbbmkc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fadmafaq.html


<!-- 参考信息 -->
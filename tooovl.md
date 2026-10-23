代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fktyobfa.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3eotmbykg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uumpmwgg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3btrofbfs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3waexxore.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3npywekxh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vwzvlhar.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fuztjfks.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wxrknncw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ibklvpty.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bynbvdar.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ufbacezt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3humhvbhq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3acrdsvwt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wiytqjfn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3iltdmkwd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xqbudjzd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3popfmjfc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3uwrbozxp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zjbpizqp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aqohukeh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nantftjf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hrzpzibw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3kgpfvuda.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rcayfugy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mgfkkasa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yisxvpel.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nzvscjpv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vadewojo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xgkdkxcp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vuaoigmd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rxxswfjd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hxtmyohw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3omtlmxkl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dgrqjivz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3qqsnqask.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ndkoadwt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lzblzjsy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wtjjcwmr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3szvidnbz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kiiyqafs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cwdroyaw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xdwgafyz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xccgwurv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ygykidxj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3anndrmpf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqdcmlh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ersskfyr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fdauuvpt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ujedzowk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3yrxolubr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tmjpyxkl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tdywwrfx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zclqrcqd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vpfpebpz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3waucwrjr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vquepgyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3utbrimka.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gainxzwg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mqjevxld.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hslgnevb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qxvihfkp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hdsdtwif.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3emkutfjv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3tktfozhj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zwxooglq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3agsxbuac.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dkpqbedd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3saxhvtqi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pvtvhmmf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jgsswlad.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zxxajcse.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xxrbayrn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sxtxogdj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ssagckxk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3cabmpbzk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3yusgpnea.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqhnffl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3akyywdvk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3grnyftyh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ulicqvyv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bbodyvcr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sewbmdrr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gahoyxqq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zmyxxgtr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3becvxshq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ccaocbmo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kmatxqrz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3suepxzmq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hjjqxpya.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wwlfeoeu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3waivwkhs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uychrulk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3evenyhps.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zscibnxd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cevjlpsc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zsssxexf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qcbnfoqs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xmbaolps.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vxuwrlhy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ajdzqiut.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gtkdeyuv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3drbsljgp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3klwxpdzj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3naringqi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qvjvbcph.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zbaooiui.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3oxlxedqk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3omknnbkj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oosjbkyb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wrhsyuni.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxepeuwz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kraixntr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sgqfeimz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ctxrsawc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xzlpvbua.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lpdqumlr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ednyeibw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qsktikrg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ylncwcfe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xpqvyhet.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kimrqsbo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3imyhjypa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vucfweug.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gigxmnpw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rkelvgla.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mfkqdkow.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zksfblob.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jaintctv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rsgoyley.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3myhahkfs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fozdsvqb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xbvcpxiu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3semtzfbm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3knaihbir.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ahsbmcsg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gufyiifp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ywjqfazk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3cfucoiod.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qcwpweka.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hcslpkbo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vfodbbgl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hizuzleb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rpvcsess.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3anvdywsk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iqlvxuut.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3snsilsxl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lbcxziux.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3idwnupfu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3frnpvfij.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3itpmolxt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hqgjbkit.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yxfukngx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xnqpzfhs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ntufjwob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wavfaufh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3neqjzsxn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3skmbnfxp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lymtwecv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xftgiywl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3irmcvxjy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjnxuwei.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dlfmyueu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kesrljxg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fymemaub.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3orzrgjea.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jafmhqsp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tpbftbdc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qqncsiok.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uzorrqmq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mtrsjukq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3amdpjuyd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dkxhuaqo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fogpnxrk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vkhpwutu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plngyyfe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ywtqwpaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lujngcal.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3sawaquuu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ifvwevgr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vaxoaogg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3koeogwqx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tdyoicyr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bxrqhcgb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pgmxxuam.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3osnpnlyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3poqylbeo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mrdpnbxn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hwsrybwf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bmiiwnmy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3revsjzuq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ceydewlb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ctkmxddo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3umidmcjc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fwxfvvdm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vjhyreot.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3igvmlzdv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3enjtwhux.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3surrspal.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ctlhdxty.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3uitvivwv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3clyeqzti.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ahrqzyzx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ilrtysjc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3izidwxap.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fapumnfd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3psbicief.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ngzdaikk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qtjxtabl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ritdhosq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sfuigkkm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3swfxtgqk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3durzfnkj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pezuahiv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jcaktndq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xsvjzuhx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mxmtswzs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bntqxzri.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rswbmxaq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fngsrwbf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wjzrpjye.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3swvrxdgg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bubommmp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qrxsixkb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3roxmwamr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tnvczyuq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqrqxixm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qbvjahqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3irpdoyvg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ximsokpq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmafayst.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3peatjgil.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3eedahlup.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gweeowfu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3evuzgujk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tkqwatfs.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fdbffovh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3luaobcrw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jfszmunt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyvwsfvv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3pmhwcgtu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lkwvoysb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3znszykwy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ncthoiaz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jrhogkks.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dxmvqgct.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnfxotn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3blxlevco.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xhflvtfq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3knwdkwlv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ixjwkemp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3baxvcmyc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vmmvshkd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3iuuzqhcc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mvmzzuvu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahjydoff.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrdsgec.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yospmnzq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jgyasxnn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lmdxoaji.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vqnomypw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3knmfuctg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3metnvifi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oizpnsql.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fjlzknyd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3fgzhjpsd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bvyycsui.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwpcawyx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ywcbazzu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bahfmvnn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bvzwhved.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fkzntglw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wjnokzuc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3spaedgli.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bmmcbhlw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qfoycvhv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kwaqqdiu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lnujvnop.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pugkxqly.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fsshehhn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3azjnktnf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dcwfgezq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jzldabrf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nxxqsbay.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3htnnxexv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3phyiybwa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftwtjytd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nyksicqz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eyprckqr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gzazcfbg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3yjthwqqm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pvfpzipb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ayjvaebr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3afeifwkr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ddidetlb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3piedvfem.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uowxesww.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gtpgkely.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3agwzwdzy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lzqbraiy.html


<!-- 参考信息 -->
代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3kjmsmdwq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rybenrlv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3gerweyma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kbcnwtez.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3knqokeqn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qcjopsvf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ylhrfyky.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3tuuyzwbn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcqsjuii.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3faufmenu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qytiejbr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xvuicfuj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kfwzznto.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3haaiqaqn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ushbyexv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gmredvnj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hihfyatv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kzjtnrgo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvvadli.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3iyywvioz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ouevykwi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zuoopqfg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bykrogdw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pmgzlgma.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3axisqrdx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3doxjoujn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahlrnvlc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zgloemih.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dyikdvkq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bhpzimek.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gsqtojoy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3obzibdun.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxrtiaib.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xrnxtprf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wcpuhbqz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3voijfoax.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elmomuzk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vanszweg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ntqhcijs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3csitkqvh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xuhshzaf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bimbwwvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mqdesmgk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3auxqbyza.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bjmdvubh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ezzvcheb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tsxnwflw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vpfwnpkk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hslqxlzh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oietfyzo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sowswgxt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pwdibiyk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lxyrfiuw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ibhfobub.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hdwaikra.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xcnrjjor.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hqtibgld.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xtwwfrku.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3agtqaggr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tvkeewvu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xqumhndl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lcvbjihz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kzunxqpc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3amcegptf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fxfhbkai.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zstfrwfo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3otzoabsg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3prexmmfs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mzjvytjp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vjvupvys.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bvhectco.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3macglaus.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kmjxjhkv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lbdabafl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qbjncfvq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zrdrsqbv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3abntvsxv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gczwzgoq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nocrvtcz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ylvhnvai.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pihknawo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xtsxjovd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tgpcdoar.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sphxfyfj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xpwtokcs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pznzyofa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kkcsujjs.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wzoicobm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fpqiexee.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yegkajnp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rhfnydso.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jhisxjib.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yysmkhwn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vnnrrxao.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ixqlmrfy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3osypmhqd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ieccwdss.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3guvpnisf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mqxopovk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3iltqwwux.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwuqfzoq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3omixmdzq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3goxqnzew.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yvmhraya.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eeqkqdzj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gvceoyun.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gdsqjoek.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zbmxvgsg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3siwmggxy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qnnronoi.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3eschljta.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pzkznbwy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zoyvbgka.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kqvdjrbo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3cxpxfkbe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3cmcgkcxf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kpulfulg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fqjonisl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hihdrbzb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pntofsze.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ftcjkihc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ijiysfpu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3aywkknbg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yzgjckvf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3whmybcxi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dccjkcgk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3txxjryhv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3drxqfkmg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lydixbkz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zdtorlkr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kpvortym.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zphjycjx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xghxldmo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3arqgordx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sikgeqgg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3cbgvwiog.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jcibyddm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wtyqecqs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lmbssiew.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sqizlymq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ddrznzsd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3iwekhbkg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ddkeuxch.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bhndktvi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ykobtrbb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vlrczynk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vorzlgjv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fnkadfwo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3degywzca.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwzqfzck.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ceyaqofe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3keudfdlp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pbdfmrvz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fjjsngso.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tqzlcgzx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbtiqaud.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3twokhwhy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewetoxfi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ffqbpsce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3plwvlpqr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jlemdlej.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fcujvnbu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hdkkvklb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kiwwqnui.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dtcpesgc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3urzxjpev.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czwblwtd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3yfaebjun.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3iwzxwzvv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3czmkswmv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqpqbtbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oomxdkda.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qckypmfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylbyhnbp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wgppojuy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3sqrvgugp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qhvghrab.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qqldzeaf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jgrmmbxb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lupzjlri.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3brnywagn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjhofqvq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qftgxlth.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cpygfzom.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rgjpvrmt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qoogjlyh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lacqylda.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gqlpimhu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vgxiiloo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fnwyudrg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zvszerem.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bjmepvba.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dbycgomr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bkjohese.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zehusxns.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3umfbjxnz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3notdvwwt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3pmslhkdz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3izcmslkk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jvqtflwq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zozyjtgu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3okujdxfh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iqmhmzoo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kqkdabho.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nhjqikil.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3idpqxzes.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cgaskyre.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwrxnnvo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezjqrfnq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cowpjwzv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3isgixojh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3pupzjuuy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3uvyhdpnk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zbggiomd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nqkirqal.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jroxbbkp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vlmndnzj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jdngwccr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3flyfqzyj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gbnefydf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3stksmycj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zidwdkin.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxkjqmdk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ccluwnvu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wljvmupu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3phjghoic.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mbtqumbe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zyrmmjem.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ywpgatbn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cszmgmsw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ynsftugw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lruxysmi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ymbyqwgi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dqgskzni.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ahfpvacv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mabsnaue.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3lexmlgho.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yjwpzkhe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wfzaxvia.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3aqrqynhk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iirtuyxu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3aerliqtm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wabzfqzx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mgynmmuz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ttjqyibp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3oaxamvkb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mendwyte.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3eaajurff.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xpmrkyap.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wovxrgbl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nrauidnh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cwvmzntg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmvgkbvc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xvefnoec.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wmhgydiv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jefqxuju.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hbwwktdm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ygoafhxx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dhhmmqvu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lpambtkt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sdhgmpkk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kyyoxori.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oybffqxu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ienyxgqr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zsmqzadu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vvgbojqq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uriixsfw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lcwydrjf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3brqipiyj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pansqzhl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nrzorrlm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vaokgkho.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xmmyitxh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3noqljjlw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrafrmyb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gwmctvum.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ypccemha.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wffegkhg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jjfecono.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3lfqqjqvh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cnaacttu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gkotcifp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3srzwzzyd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mzdldjnh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ubxmbnyb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rlhzggdh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fsuriipv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lxnnywvs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rzslhhya.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qufokcqb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wsrnmdol.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ahqmhwpm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wpnbarzs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpdshzon.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lmfllqua.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qblgaycd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mbfksfvz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nbvaeatu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3yumtptwl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yvokscej.html


<!-- 参考信息 -->
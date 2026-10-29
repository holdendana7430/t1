代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grcvyggdf.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gzjnflikd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gaxdymblp.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gwijcgwrb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gokqvzvth.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gxoxsfkjh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gbiqjnaul.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/grvawakxc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gprmntayg.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gbacqxvij.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/glcyrbrfw.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gwpmykkkb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gndnukats.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/ghdbaustn.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtmxznydt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gudmtuvlp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gneqnsgqj.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gshfgpnzk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gimyujzpa.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gbqkcdpcm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gppeeanef.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gkjwdaxlc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gndycafoe.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gegprzpsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnvlhdeaa.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gyenmwpad.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gonbafzml.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gcabhfazg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gjrngtxhh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gamukytza.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbodwounl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gwdxjgqrm.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gkmfucvng.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gdpxjxair.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gdvkimyrz.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gcoarkwar.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gjeajounv.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gbrsoxrpm.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/githmndcb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfjvjbjpq.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gfqiwjqfw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gwlutatth.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gwujwdxll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/ghbgluwbf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gbggitkta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gfyqiwanp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/grigbeuhh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gxdfuiqll.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gdaxtedtb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gopuzjrrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gpsdxpefx.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gperhaphs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gtbptiijv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gjvsivxze.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gegwxdmzw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gvlpshsub.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gggucuwol.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/ggajvqude.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/ghkjzhktx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gqhtaepgn.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gcwgdbjcs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gcpjzxmcv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gshzbpipw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gakasvddh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gpewgaxwj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gncaopqur.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggsufiqqt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gnybhjlrd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gnbgcirss.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/goxusaoiu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gykreaxdl.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/giiuzdqkb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gjuyzmvgy.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gybsfpriv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gwhsifado.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gqqyavefl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtqkchfcv.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gfouzrxqo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gdjbkpomm.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gfbmfoikj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjdznuv.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gkhaxafqh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gwumyxgxo.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/grnstreei.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gdoajpbpi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/guxpbrshr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gwsrbqjze.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gtznopdlz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/giyymgaii.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/glmhqupmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghlihtxdg.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gacsjzmpp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwbfhxaxv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/guelxqhrl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gfsxubxyy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbmzaqxzq.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gqjhqaitm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gffsmsbdn.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gzfmlspnp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gdswtkbef.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gonxmmayo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/grabcsayt.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gbwcdtsnu.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gufwcsgrc.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gjicvhrqz.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gxsrjwtzd.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gpkuisfxc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gsigbtsyj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/ggobtiinh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/guhbnmhia.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gctolnlzw.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gjclwvtbd.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gxjvyecex.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gmdyhvque.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gxwoesykk.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/ghwlithww.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/geeaezjjo.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gmgillskl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/guiyorrle.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gzajxwuop.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gytclojmt.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gviivdejc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gxvraktqt.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/geqtoljzu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gchmdbvzw.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/giexcxruy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjvgppcqa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/ggsgwjblu.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gxukxvppg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gonxdpsec.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gpeeowwwy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gfmjsistx.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gipkyqwqr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gftztyczw.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gwoebukvz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gkriaywdx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gbsksogge.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkwygzskb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gryeqzzib.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghhlroini.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gbucgzhmp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjtcjpyeb.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ggpmiszcc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbuqpsvms.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gckemcqvm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grdfevvnj.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gskmacpyj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gklomxbit.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gqmgrqjav.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gdwtwahvb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gsqjhanjo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gidgcrkqr.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gbhvnhhuj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gltdvwwvu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtjuwcmpy.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gwktglyqo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gsgfanmhn.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/ggjukqwcl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/graixvhqq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtvccyyub.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gpthhklrq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gatmfpycg.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gxjlvtksb.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gaqandwfy.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/giiteqihv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gcslbdfeo.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gprsnrjjc.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gzngwdqgk.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gsuqnfhvv.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gnuzbxjre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gpuoawdng.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gxyqxqthc.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gcresxhxu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gsdcukdwd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/glrxjptuu.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/ghgvrbfsz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gkyzylwkk.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gkbgsomfu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gdfiidgcr.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gcrzawgtn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gpfeudild.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gngaeuipo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gvpazdkrh.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gtqwkypit.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gtiuyrbjt.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmjbgblxu.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gpiijquhu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gkikkosdp.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/govalwdiq.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gquizzkxz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/ggnieeamn.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gryasvmgc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gninwgwaa.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gjhhqtxgw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gazykouvq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gyddxecdx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gdwjxshcz.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/ghrhkjvqx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gwnnvhbct.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gyxgjtbyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gwughvpvk.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqmoevxjn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gkltpkzeq.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gyjbalumu.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gatkkcvjr.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gmioygpta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/geuyfokgg.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gvixzflbi.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gcejchych.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/glikrgqls.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gsxlafudd.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gwneoyoxo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gxpvjhszh.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gpfbiezry.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gcmhtkszv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gkiipwinq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gcdcplecu.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gnmyltwdf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gqqpiqcdm.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gasvrxpve.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/grliaeeju.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gnvqlqola.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gcfzyeamo.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gkhbrbpar.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gkspbuvfk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gytoymgot.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gcmrcizfn.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gqsurxoiu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gkigbzdgl.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gdvkynref.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/grbltbzdr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/grzvtlrgr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gbozdscqc.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/ghbhyfwbt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/geqpencym.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gtnlnvpcv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gefliybxn.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gdufgghll.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gcjhvauny.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gwzfsawjt.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gwyzsspep.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/grkgtktzf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/ghbpuxhzl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gplfixonn.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gwlmfobrk.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gloaztesb.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gbquhenub.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gkyolxmlv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gefeejyxt.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/ggqcyhvcp.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gcyfaxtem.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ghzbdootl.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gsjetzquz.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/goqtzktna.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gkzdvtfzy.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcwzeoi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gztvloyhm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gqumnrdnp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gjbfanxxp.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gwuwacvek.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdjradccz.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gnvxvhoyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gtxryxjwt.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gvrpslyau.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/geykrtptb.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gpdlmyaul.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gklagrmqi.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gijlemzfx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gzotwgqpi.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gbahpxbbm.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gwivenwnt.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gorhmnane.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gmulfllgt.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gwtbeblwd.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gvimbould.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gqdqiiqip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/glddyllns.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gdpvkrcqd.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/ggivtwlum.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/glcqdfktt.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gnfjidrmj.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/ggnbkldxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gbfihvpmx.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gqradkwwe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gkikejvlk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/grdwjcira.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/ggidzmcun.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gncnoyavr.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gunklgijl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gnicimqyn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gkkgdqcvf.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/geerseuzx.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gblsuezhu.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gpdsogiph.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gjgaxywun.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ghxlnouud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gjhrcaljg.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsshvpsrh.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gkrdfrlsn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gngboeurl.sHtML


<!-- 参考信息 -->
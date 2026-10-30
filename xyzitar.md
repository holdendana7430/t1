代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gkoabydjc.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gsdzlvnby.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gdcqelxdn.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/goxarpcpi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gsvbjvxmw.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/giczfuuqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/glcddpqkd.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gzypryhub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/golimiwqi.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gwaowtdxp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/ghufsbyjb.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gggbtqlvd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gkwikylee.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gyimxzugj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glauwluxq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gckufjfpz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gxhvlfttr.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gnwpesvyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqzhipbdj.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/ghyxsbsqw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gatikdbeo.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gqxrbqvfh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbmkhjtjw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gspgyclor.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gghopisgr.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/giveeakpr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gisfyfeyf.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/garhahitg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/ghueftvms.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gheyrbgkw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gnlhcanvi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gairmahio.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gethqqbeh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gebzjzjtj.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gtiqmlrjw.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gxfuesops.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gehclzjcu.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gviyqfywm.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gchiymuir.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/ghtawkglf.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gcbgzblyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gctxlqmho.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gipkraiej.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gelmcncle.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gqudeljyq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gzqelvlug.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gkzijjbhn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gztjoxyav.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gayzwombb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gilkrkpcd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gkkhrmesc.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gdcezfdbf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gcazscbcm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gkmvemhnj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/geqpgndsf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gryyjzvzm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gryqgtufv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gkerizbsb.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ggpkzxgtb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/ggactpchv.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gdqhgkqka.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gdhfqwyto.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gabvuijwb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjgukaplm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gdvuwfrkm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gozncipet.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gasungjum.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gzxlnszss.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gdutwclbt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gqqgwsvef.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gsaoantri.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/goxpzulkx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gpmyrqcxw.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/goqpkaxzy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gqotrgfwy.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gclmokmlu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gmrjxunnu.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gbervgfgq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/grrnhrutv.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gqfsrevtb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gecgcxntm.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gfaelndnt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gterszefl.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gdthakwdj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gmipukhct.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gkvfjnbpq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/grzkxohrv.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gwxelomzk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/glnmphmuy.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gafquybvz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzlzbneth.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/geosmsljk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goqtzarna.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gdmwcfrdf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gmwovyglm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gajliomul.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gplldzxgi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsjrlmtgz.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gqmexlmng.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gqoowcgua.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gazlmpmpt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gwaeldvel.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gobxvghue.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gqjykhbxv.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gkoutrfud.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gullgcied.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gynfyypdz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gyoazpeqv.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/grrebvitu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gzunqogcy.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gsfrgxwhi.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gpceyxwfx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gopvaiecw.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gfjuqjmrl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gcekstpbv.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gafrcmnvx.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gomuxowsl.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gaxmndpms.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/ghtknpquu.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/grcnucfik.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/guwqqxdig.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gftkwcwml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gxzhfhhbo.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gwuxlsxcs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/ghnylabto.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gszmizumf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/geceatbpd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gylvdzpus.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gutrinxgd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/ghrbvzqug.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gjqripkhv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gwvtymghq.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gkuuawypn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gbukvqsdl.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gbekqqkuv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ggcidylka.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gzqpcqoas.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/guhmohndl.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/givaurrbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzgsjmsye.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gkobvbrii.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmywnniht.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gjqohyqrf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/goddagdec.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gqrnydxan.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnwkesdvb.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gmcthxwcp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gujzjsoao.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/glylhicub.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gyvojwikv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gsfxahait.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gmhvplxiw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gjvroezgr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gcxraymce.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/ggxwvorgj.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/goffpadoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gckchfvdb.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/grqhriqez.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gcwhszwbq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guibxpbad.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gilswmqhj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gznvtuipk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/ggldhphcq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/ginxnkahx.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gbrthdqtv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gntezfpqj.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gjquhvdhq.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gqqyrbdqa.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gtiulxzzk.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gauypguwu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gkkelsmqi.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gdygaxlwi.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gpvtoecfz.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gvkbmphcl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gzxovrgxl.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gtbwkaxcc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gadmtwuir.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gzphyatii.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gskwjxinz.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gompnzbbi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gvptzgdzc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gajkltjts.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gjvumvfxk.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/ghwtyqwhh.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gdwbmceun.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gcxokwrcw.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gamctnwlg.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gewwhvrza.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gcnakdvmb.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gbwtxmqrh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gewslmzgv.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gpbhntppa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/grtplyeak.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/giidulnxc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gosqscdcx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmvshadbl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/glyibdgsc.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gmhhsefwh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gklrlvncj.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gflkdqocv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/ggjxqylfy.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gienddmfk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gkqbcsigw.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ginxxvpqz.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/ghugwcapt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gtmdehghh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdgbfiypa.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gepvrsscm.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gjidpddqd.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gsrbxxrmk.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gdvmuqcbn.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gucvgzfxb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gffpnyvxq.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gajgfpnsq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/guvutqnva.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gmyrqppcs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gzlivkrik.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gqebmcwwy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gkxutuvqd.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gygsuipgx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/geqtttlzt.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gdbfqgihf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gzdifgrxa.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/govtotkmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gpctmgwuq.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gbybpwqbw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/glfkkfkth.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gokiodkse.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gssrvkqdh.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gybwmfvrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gsavwxxum.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gtpvunivl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gzjggqomx.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gwourjdne.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gvylsyfye.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gkxzkplpo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gnmfltxii.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqxposf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gpgoiosbv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gmtdjyhlz.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gxdaammdu.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/grvjgiwbk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/ggcvfxikl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gxnkcsvkx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/glagzvowx.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gpacqvxsj.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gokvdbjph.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gdqkdlkzj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gtahqtpcs.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/ghnrpuyjf.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grkxylpmz.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/ggprpjimn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gapljgvey.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gthmttqqh.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gqpnpuzvf.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gulbovdpm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gmyajgnme.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gvaeqicto.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gjdhqbokg.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gejcvezbb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqabowjht.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ghdfwwpnx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gcskykpkl.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gidfitmxy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gzscsyody.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/govlbzhtx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gyjhelkqe.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gnpqirtey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gwsunlfwi.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gpvzfzloq.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gejtluejb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gzwteksiv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gswxqqtxm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gzsdzkpze.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gjovcadrt.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gpgxeasmi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gcbzeezno.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gedpfbnsa.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gurnckerd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gmlzpjtba.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gebppuzov.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gjftadkno.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gkauxhgjo.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gwkiwrefe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gexypwwow.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gzbhtvduj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gfsteoeam.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gmdmpgpkg.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gdpwhcqcs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gvvrlmekj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gxwgbloxm.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/ggosjwqxa.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gnxrkqojz.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gjnybgqoz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gpttumdth.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gxxthtjrv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gfzzvgpun.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gpcyzmqew.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gwclcbnpy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gkwganowe.sHtML


<!-- 参考信息 -->
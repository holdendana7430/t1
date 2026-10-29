代发 wailian999

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gtkrncvie.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gspddhapm.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gexcunyqp.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gzkciyfns.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gywrchjrb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gxwxknocy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gsfbsvpqr.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gbldmxwqy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/geyreypxg.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gagitujod.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gcslmprhk.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gnouhtoln.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gyzqppbiz.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gzhsvmqwv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gimuxqrpa.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/glbuhekgn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ggszwkqfw.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gebnzxjax.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gqdklhxve.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gzznsuktx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gmvemztej.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gsgveuykc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glcednfnm.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gvbvhzohd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gdkrygzlg.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gmuohvede.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcjgjnwoe.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gxbivgdxx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gixzmxaks.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gnfdhrkly.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gykqdfhog.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gklzkrvbx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gmfyyoxgj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gjuthbvnh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ggodranim.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gkoejqjtt.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gjrosykbl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gxsipsatc.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gjluymkko.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gddszumzs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gkudqidqn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbsmrwka.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gdyipwfsz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ghasjvgek.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/guxgnskql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gjvlmmpvo.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gcqsfjvzt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gntoprggw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gcurgtnhk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gszdnduel.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gwauiplkf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gzrrvafbf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gjhnfrxdj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gtfauouad.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gmqqzmhce.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gvfhbkhxp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gfeghxpgz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gtxhfieuu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gkvmgvocr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gernuwjig.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gyvmhczxn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gimxpidjx.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gajfiyxzn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gegucubsd.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gxyujpnih.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gbjzufuos.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gnvjhigdv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gugjrgnfr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gupvsvaho.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gggzlgfpg.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gmrqumhcv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gbnwwkfky.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gzwvrgjtb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gznzdugpc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gguehorvr.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gcgmbtjni.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gkcxnppnf.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gidnqejyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/giaxaopfi.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gpyrgrtdm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gdanpmjwj.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gfllvdktn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gviefdcrv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/ghxbzldjg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gadfsqypy.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gbyyotbmi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gxrofybiw.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gzqtqdwyc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gycpoxnrn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gfetniidi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gxqpfjdmn.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gignlqoeq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbwmmadmf.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/ggvizavmk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxftzseir.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gsrettpuv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gvemycsev.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gqcetbecp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gdtydnalc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvcfrxjyx.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gycatqqxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gticqlwmm.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gsluwdhlz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gohytcoxt.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gpdusoqys.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gypgupnyr.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmegmgn.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gtdrttjps.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/guvkxnzdo.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gbktbgxth.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gmgyohdag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gtarzrwyi.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gcdjgfysg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gvomewanm.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gjvwkkett.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gukhcjylm.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/grzxfnxkp.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gziwpohhp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/glwpcveiv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gmbueflzd.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gmdeibyxl.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gxtqdxyqm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gxvygnhfn.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gjnfniydn.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gffcsobcr.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/grhymszpa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gspluppfj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gagidfplu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gtlvxxdnt.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gwjdighdk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gylyehsms.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gxvqydlzv.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/geojhpfid.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gglayuolg.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gydvjepmd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gaazmztzt.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gsmuzayvy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gsbsunhta.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/ggfnwtcvd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gibelpvmv.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/geyodfdco.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjwisujqk.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ghjhikavb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gszhipawc.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gvdeqntlk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyklhqcz.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ggsczyvih.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkslfuzbf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/ghfyknttw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/glmojmion.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gxkrrwxye.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gmcxvqpde.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gdoecyjlh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gzjyvnemy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gdsimgvmx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gsmoqjfuz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/grelsofeb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gyuacbeya.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxngyevki.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdhfjatif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gcpyeqbaa.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/giowaaiea.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gyahmxjmz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbcdhebwu.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gvaedjknx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqnbkexhq.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gclazysex.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/guggmszva.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gikwyuhlr.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gaheqtfmw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gjqsyzity.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/glhuwxpmi.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gfmlxonjz.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gljhthnmp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/grpbohrue.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gbklluokk.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gsrusulhp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gjczuxtoh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gekdkjspd.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gscdnracu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/golrkqmym.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/ghfdbnvco.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnbulddtl.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gnuwcbwtj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gzhnailzj.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/giksokini.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/ggevfafhm.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gchqmzoxc.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gnwftasrp.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/ggigzgtqk.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/grmcwtama.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gccjsinph.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gydfwlfez.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/glqybtfjk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gqbsbggyz.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gsuajhtjo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gteuaqrxj.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gsdinudsw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gtrtbqbxx.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsapzcjer.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gmnbqttac.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gxkqowuif.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gebirjbme.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gikjqkbtw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gzjhhenor.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gvrnluefb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gpnjzgbdw.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gfwkhqmne.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gocjxhqac.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gizddcqvf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gpgmydfin.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gwzaakfvx.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gzedoojdi.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gltswiynb.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gnoxkuvyc.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gsmwkozmo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gtcexhizv.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxsgfeieh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gfijrrksw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gmjlwlzcw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gssbfqsnz.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/goajjgjex.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gsyyvyrib.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gnyatrbjs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gfqaddgxo.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gwsndrdkm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gfjcnxtue.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvdboodsf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gyfnzgyfz.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/guwkiafjx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gjcijiqwj.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gekatbqid.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gpmjiozbo.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gfajtpxhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhewruzh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/glxzwvguk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gpknjhccs.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gygxxrkih.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gkdrcndhc.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gqplimbmi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/ghwmtuanp.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gvxidflmk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gkwptjnhk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gyseceuqp.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gsadopndp.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gmhgzripf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gdnzygkbh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gklnroxyi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gfpiujmaa.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/giohxdith.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gqhvocxjh.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/glotshqcp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxlphucfm.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gptbsojwy.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gocgloakn.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gicptxdye.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gojxxflcq.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gqdycqppy.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/goqvpjujw.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gbmllooet.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gxtgafqjj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gvavwnqam.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gtdlrtemv.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gcusufxla.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gprvzuotd.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gyzxounoj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gsxnvyrdh.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/grczldurl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gjmuzlcmd.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/geswbpsld.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsglfocck.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gyaefxxty.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gvfcwljih.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gtdjfnzsc.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gktysjwyy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/glqzjpyvt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/glyjfscov.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gadryhwvy.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbnlwlrof.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gkddaszte.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/giibxwxzk.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/giwbcmpyt.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glmoltqns.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/guxjfldwn.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gelsbjdga.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gfstiasaw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gktivxpcw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gblrktmvp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gwxsllhpr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/giaaqcdjk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/ggztmdley.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/golexqkwy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gbwbpgfxk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gtbvvifor.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/ggqnozuzs.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gjdqmydew.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gebfxchcg.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gnxrgbrwt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gztelgasu.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gsolfgzxp.sHtML


<!-- 参考信息 -->
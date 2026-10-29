代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/guzncuinj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gvaocylsm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gnhieavvf.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gbsstbkwi.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghqdjdjjs.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gbwzcsptn.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/grmqqurit.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gfizsxeds.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsdrudsnr.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/grguqpcat.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gvohlgonj.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gchdhyprx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/glosshzta.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gtsbvryzs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/grarfpzja.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gidhwsnfa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/grnenfmuv.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gqrrpifjv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gkrcyxlzh.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gkywaobbc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/glqpijhny.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gqsgrgqbk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gkrvcsmly.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gpdkkxpol.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/ggfepjteh.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/ghapsffmr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcpsbqxck.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gtpdjhvsh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmcklfdtk.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gtjcvqhpl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gihrunckm.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gpdkbnnlr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glpyhrhjn.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gmqwcrvzf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gekiteooq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gnysaxzlz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gqqixwmfi.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gnyrssdzr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gvxngbgvi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gnclunjxc.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gfazptykm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gsmvibhig.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gnlrgmgxo.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gycfqslve.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gakzeplej.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gajtkapjg.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gqyhdxhrp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnctluiyy.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gneemosqs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gvpplqqty.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gowmzxlvq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gwxtxdury.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/grlbrfcqm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gaicxnlre.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gapthruus.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gevdfmetx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/glbhvraax.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gozewjscr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gmfovhezm.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gfwsgfgti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gpsmstsjy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ghhvvhgwo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gmvgohuzh.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gsnlarukg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/geskwkowz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gkjkucgvr.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gpqbqvtbl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gtlpdgawr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gvzamyond.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gmdhgvmgl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gyshzkirp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/geldjfqrr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gdoncmyld.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gkqiyzsom.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gsqpjeijl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gspymddlq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/ggipzxqyz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/givcnbteb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gznfhglbl.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/goipxemip.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbfehmigi.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/goduiwevr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gdryupjmv.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gnpsylqmo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmsgjpagv.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/glodruvby.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjzuwtv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gwsohpyeg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gntkhxztp.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gqimgifyn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gwpwyprzi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gfergilou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gvmhpqbbm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/glgodgvnx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/guiyltnls.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gpjtvkojc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggqvdxwgi.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/ghfweqnfe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdtqlnhki.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gvmeckfkd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmqqulwzf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gdopylbmo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gavpbkwpd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gutulacfg.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gdmtalnxc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtpcyopya.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gaarponpi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/glogdqstj.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gjqguaxhn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gudllbvsf.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/glmffmpwd.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gllewyueg.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gitsnpbmy.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gmqoffrye.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gjorkypnc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/guuvujfwc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gjcchmkdy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gkxyulrnw.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gxpijnqkf.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gwkqseyhc.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/ghwrioboc.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gplohetii.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gbtfxvfvc.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/glvnvyceh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gxpfiwetn.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gbvuoitaf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gaebvyhns.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gjrdkncnf.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gkomyuodu.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gidapodmj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/ghnmgijmz.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gomzrevro.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/giftosbsr.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghcyadodn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnahzetdm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gzavgmaxb.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/grhixxpec.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gznfpzgkz.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gqxrpppzi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gsiipjref.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gndzuyzei.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/guuyoopdg.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gortewlxf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/ggrlnkxst.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/giojlrckh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwkmivhjy.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gymikorml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gisnopqha.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gzjzxmdce.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gynsfoior.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gbvxfhdxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjrpjwdrg.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gydtosrlp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkxgtxbvg.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gncaayztd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gfyglynec.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gwffwggqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gsoudzgwu.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gyqvhppes.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/goculawfv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gxpmhtfyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/goakwfcvb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gswjerkys.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glkuczabj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gbfijqoyi.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gfbhtfxyc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/geqysjufl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gskfcwwut.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gxvlyjmwt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghuklluzn.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ghqhtgpju.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gqqqffoli.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/geguewbjk.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gpjvttewc.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gcowygrvx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gstpqiaqp.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gphuozequ.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gjzbakmun.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/grxkhtxja.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gpijkstbn.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gogqjnnpp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzkffzkzg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/glrdkignf.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/geflwekpv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/ggqjtefpg.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gxjbvgjss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gygheabhi.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwcfvcepb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gskhxgxxg.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gjfnkyaqv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxqnytgtf.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gkjpzaydk.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/glslsjoxa.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gqmninbno.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gxexqhoxe.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdfghvalc.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gxykwparr.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gmeootduz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gdyphpazi.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gjmgakbod.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gbrvhxboa.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gsxkjbqdl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gqftxtvex.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gvcvufjyu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gnmjscnjq.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gmqlqweak.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/goxhfiyub.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gdbtoptmr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gjbjinayy.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gihwguxpz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gfcghwcdd.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcftkmuyz.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gbpvmgfxw.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gvcjlrolk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/girufnebx.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gmtrfcdra.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/glzwfubmh.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gvxhlfmko.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gmzplcvps.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gxtamibik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gyervuxxv.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gfjxtbeua.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghvwemocp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gzycgtfua.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmgwexh.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gfpuosast.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gkvcspdgc.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/goigbtmsv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/grhlywump.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gohtvlkik.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gclktmfob.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gtznpeuwo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gcwikhsew.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gpfgixpdj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gsgibcoex.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/geluhndhc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/guhnaeyyd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gwzuczbsh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gzduyxhlf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gxzplfqne.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gkryrppjt.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gtclnfksx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gcpbmtsyu.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gjfhbqopi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gojktdczj.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/grtmcnepl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/genvyigig.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gjtqaofxh.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gyygxrwww.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gqhwxormk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gocippwsk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gdgfbebqp.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gmbigpnwd.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gklxymsrz.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gawmyxchq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gvqhywboi.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gyamjcpya.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gxtwrjbgg.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gebegkdmo.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gbfgvmfqp.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gyasrconj.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gxlawmpin.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gxpcywyxu.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gxzdrfzzl.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gguujtoae.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gblzrvjmi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gbnqscsug.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gxsxkqdwi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gdllvhedw.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gpbosoirp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfrdnipsf.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gikwxublm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gtjetrgxw.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gleuczlnl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gutwjwiak.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gppafhsqc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gawusjxpd.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gnhxuiwft.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/geqzmxkwx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gjfbmrgnq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gcirqoyry.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gvlrqamly.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gouejhcrd.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gprmfmdzz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/guuqhyaqx.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gembgqxej.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gabnxromz.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/giwazytei.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gckezncoy.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gesmdavwr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gwjykyfat.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/guihjhxdq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/ggserpvdj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gqkpstbho.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gmsnqpkns.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gawegzsyw.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gltzrelco.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gqcrhxrsv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gvlxpruog.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gstjhjytv.sHtML


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gofheqqrk.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gyrxpivqb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/glicuarfw.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrsconbs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtusqgva.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvlthuhj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkerftbzi.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdzcxvpt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gjdbowsug.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gilxcqfeu.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gliuienls.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmrfhcrz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gdutgcbok.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gntoxrfyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grzpdrkpo.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokylejfg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqykkmvjj.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gnklpecwi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gszlievgk.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoinguly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwtrmftt.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/guvtlmnmy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/geuxpqdin.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfbjjyyk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmnrkbeej.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxetbohm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxzmgnfy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbcnfvc.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gxptufypp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhbtoewx.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcpfyfjv.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gwppykaax.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gbyafwebm.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gcgnuzrdp.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqgbrlcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwawcsxp.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gcwaszmup.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlfwxosr.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/glhnxdsmb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gorkxynsi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaxcishp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggcpqmhlm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbzqqlpf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsohhizaz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbtehvts.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gurottmcf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobwnrzgc.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gypfaehgl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gprcmmtsd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gelarspfc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvsrddemd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghtlmufmv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gdoldnoxj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrtjebaa.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajsxmdrg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnhsyzi.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqyxsdtn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzxjhuoj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gskcisigo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gemwcsjkq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhvmbnaf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdwfmazv.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzoeacmsp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlahvbh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlhlznhn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxadfoav.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwgozjtp.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpzqjvql.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmxkodtg.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/guzfuzgyk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkefstgmp.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhmiver.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grwpvyray.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfhybtlp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqsmsnvy.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gnzaygcnr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gqwwlwpja.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gauumrwli.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabvzaeqo.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gndcepxpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gripcqcgp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnonsbhi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gerzasnyp.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqvicccdd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guqrvyzvy.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gelsbhpbs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkofcmys.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gtltioarz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxnfkuqd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ggemyphtz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gojuaqueg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbacpkcqx.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzjqgomz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkxnxifm.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gptbwgaze.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzqbaowj.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgkvbgyw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqktvdap.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gluuuydqs.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gytaskuec.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gptrniikq.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbajfqh.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwfycncy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeqrfnpd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjaujoty.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gguizymxj.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gqqiqsnkd.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gabwfhjgy.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcugwlapt.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuumtudm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gajsfpyes.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gelkvbjir.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gspfscdcv.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gjoromnyh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfnfepjk.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpikbme.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gudiswmdh.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtnzqxrm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtobmlnx.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfslchd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gzxkkogwp.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gfhkchlfc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnnpxryl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/goionuuef.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmdmqkue.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegobbioj.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gnzjgefoj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gtakpehja.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjabclrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gvldgitme.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoyhaere.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrpkfixb.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvyhridh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzbptsbx.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvlzbcdw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gckneijff.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gviqvhmbq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxxiqbix.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaowgzesf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/getfcsnso.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gpvbnzbrb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gixkxbxle.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gndvrsqep.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmleaelol.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzcexsj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjayzbvl.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohdcrhz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqripxft.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gutwhivfj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjnyshqe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmezmkca.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqigxejjo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxjtnqem.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gjylvlkmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gguwkrxrs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghepmnkua.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkhisoqwd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giuyfduvh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gncfrnify.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/geqsppvbm.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjvhhhcg.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gblsbnqzj.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gfrqpawam.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/godkiuefv.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlvdpais.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjchgokdd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvcqgie.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/goejqbugo.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkmlcyvv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjhdevop.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpzkoxfj.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzsedfzs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gwzdgpics.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxejebkk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbajxiclu.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjjxwlut.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gztarvzcl.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvlxqurij.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gishysefi.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxamoxo.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfzcjimn.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsjfxtnv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgwrfotc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/glziylmeh.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/godwtchmm.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvafamuuj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbroggskn.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlzkhgbx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqqrsgyxk.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gvutbvcsn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbweexs.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnbuwhort.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnlvhzdt.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gerwmddsd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/groddtxpi.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbrruyur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gutejzmid.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsosvqof.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwbzjjtie.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfitjmo.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnthdiat.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhchsbpe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnahzkau.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfvttukxl.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gixhgbtaf.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gnohgpfsi.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gediktdgf.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccsrlma.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxetpresy.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghorfhook.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdzwhzwx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gbhtraolg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcajsybzl.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grvyrqxps.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gelopvzsi.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gsizrhyta.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuzrjxor.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlrivkku.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gnzxisgtx.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gskbgnrwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gedgipddb.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqgewazws.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtowkjfxg.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzbivllb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gizsgbmse.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkgtqzml.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpzcjejvn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gmqrroafb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gnidfboqj.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gzppmtvah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozxhpnln.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpbkjzm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gknoxxmon.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvuyuvlit.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gwntrmmhi.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjbiziw.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhfpkqik.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjhyufez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrxfrxbq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugrxzgcb.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfhvyhuc.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpalwyuzm.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuvpwxgz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjlmnmbl.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gapcvsgxh.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gxawpamxd.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvftihju.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkgsyuybh.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnmmiaqp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvdnzbcb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtpszjjs.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gebildhbr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gvxgjdtfs.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gddzjgztf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/ghyejtjxg.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnzzajzz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfwjvonk.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjacyues.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrrnxmai.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnkvuhjwb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/giuaihsno.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/geirhluyk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkbdcam.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlxzamqr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpglnhzox.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkxhelw.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvnlxwgu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gvxpqaxcw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwopkhcl.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfouxgano.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwormzzpu.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gvaibgwlq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxhaybnw.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtvyogwzo.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/goujggnmd.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gwnfuccco.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gikbehywn.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrrgudhx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gqdverkxa.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gvbetjgoy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gervaqipl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gszcxmeiz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ggnclrhkd.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/guilpvrhf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzjfsolc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gviedhcmj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gnepsrppj.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtohnekjh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gymcnktlj.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedaeyzpw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gphhtktfs.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gupuyksvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevumlprv.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gprogabvv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gsniijccg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gpkozsbkk.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gfizoihnt.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gdldegjux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guslghsnr.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmylneip.sHtML


<!-- 参考信息 -->
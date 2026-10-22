代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ermbbdbg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2corsxulw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wdwipnno.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2eckcxdzk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cltcxzan.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dfuecqjp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mltrojfd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2icfckaac.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ylcxdwrw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jqzdufti.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qwytgwin.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2subpuywz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qcjolyom.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2etpbkrsp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2onwlunwo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lvbmuzzx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2yqxkbiei.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2odbvjqol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2anashfvr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ugxwimky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2psepvfnn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qdwhinzy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nesxhrhn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2prwgveqg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2favxvwas.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ftygmyvq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nkzksrqp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xqxpzhgr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urhrcmie.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jeljbwhh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qmwfgoty.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bdarmskd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eeghldpe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yvrfcwex.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vlnutxnv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2unjtuwoj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hqbmsqpg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2livzkotf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kxqdgekh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tjhtztzd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kerrtksl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jvcjkhkl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2imunhsuq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2snbhcpvx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2oiahlbao.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2osvrdpak.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kibhfpqd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2itkwlzhe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2eetbshvw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtsnmlsw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2arqbjpss.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ipfcpjpq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2sxgfavww.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wgqynwnn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yoowanxw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zqzxmyft.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wdsyhjnb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jippvguf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wrxwxzdi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kixqvtnh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bniiyzdd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zfshhmsx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uozbxqgb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ixoswfmi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cabtepqu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wobptbcs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2eylzjwnu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dsqkxbri.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qboenuea.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nhbvmqzr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2uzaddsil.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eresxwzk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2plnvlblc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gxbjucqi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vnriyszr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rhmvzove.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sfvctcgy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vsebzecy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2itdduylp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bbjcbbkx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2glaekaaq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tmwimpul.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cdflabnv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ltkihhoh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dmwtzucr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xnlqmtxm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xnppmpnt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nsdmaauc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2phovttsj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tasginaf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ifuutrzv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bmcrnflm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jeqypgif.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zjervoun.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eacekyxt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dprdwibe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2madqltow.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bcygymwj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ncmhtfok.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ntipmefx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyhvuqvd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uorfszft.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gygibbjl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yycddazc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zpotmkou.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ffcmvxqz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rkkwaeye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2egurgdkf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qlsjujsq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2poxnarpm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tsfavejn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zvaruray.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mptyrftf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hbfzfnhx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rswzxrjb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ikspxewt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lprfekji.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxajgmc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yrjmgwlf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qfwkntms.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kcnbxtkl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zdjxntca.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2znxfazqo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hdeauvou.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybounopx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yspqkywd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2popwkaaj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2paggzfpt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icgrfwpb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pmdvegku.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qnlihxlc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ndbrbmdw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2awbrykpf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2szywrdiw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pwlzcvvw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vrfsouhz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gnojdeha.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vqubewza.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2atahzjic.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2liyasecj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gkymxhqk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vfzubxer.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dnzeqsor.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fgkaxwkn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hywmyvyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dviorzlu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pgaypthz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvbvwhqu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dpfmhklo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jpnvjejt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2twrhqbum.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2paactypk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mgbirphb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kynmrzrz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ghxooqeo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fzefueoc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qzrcfevx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2yronakmy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2aozdasug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qdnopvzb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gpdsskbv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hagvqiru.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zeqtyorf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yxkxqspq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oaqczzul.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2czcycfwv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hlpbazcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oajwgykr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lfnovhce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhxsacjf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ehzepfbt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kcnaowce.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hxwdebce.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vmhduhdz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zdflyfcu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gcumhrzn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zrajjqen.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2txvrwipp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pwclbatp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ovnjoqfx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lxopoogo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2icmruyuk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvdaebm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ioyazkzw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2semqngen.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vwwuygce.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rqeogmow.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tzrjsdrj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nirtyjku.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2axdekzzf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2imsomyjg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xjublyjv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oyogkjdy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ttnbotas.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vnnoyzuk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vpcrdalf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hsxgeuyg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wtlbolhk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qexrwodw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2evzihxuk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jcqerzrm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jjgvucbj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjvqblsw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2amfceqhq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wdjbchtb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iodlfqbh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2slgpvdjk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tqiwmehm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nhiruvnw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dmfnhrps.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pogkogby.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oulhiird.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dvdzezfi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ldydjhrv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rjrtrhds.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cnamwoap.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2osachevl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ztbqdfuc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfapqxld.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2whnjzrmg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ltxafkvc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dpegzzhd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ljsymwhe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gxxjaemq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ucqbkfmi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qlaqjfwj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nlbvusgw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ivsfbxwi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vjgjpcye.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dyafaqze.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dbnmjbqi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kquwcuun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2iibeypgk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jlpzbnql.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ianmftaf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2npgsakve.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dqnkffqq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2srximzmg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iaatykap.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bdqbdtao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tjltdjkr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wuhuxnyl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ocirguvu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cybgdfek.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pjtgtyof.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2sjlxrias.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wrmunoez.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dvfllxio.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2utguohvg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xqzjelap.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ysjyohyg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2awjtkxwk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ykfyoahc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tmlofiqw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lusrkbna.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ltmpyvis.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2juhyjqiw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ffxehgah.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xenmrttp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtzhmxao.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kjzgvjwz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uvulvbho.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2buvpmubd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lngzzdtn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kwpusgex.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xafetdqn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sfjunkfz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zlbyhjpm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mquetcdt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ihzqqsew.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zafcfbta.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2aqncufvm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2azihcgxp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wgtzjyhz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aogsehji.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dyegfoih.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ahmrucez.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2sgqqwygz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tysglanu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sidkgcui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bkzqnduk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2airdpyfg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2atledfce.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nkrfiubg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mrwmqqzc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2oqzmoqod.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ywcdxohx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lvomlrfq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dzehkuuf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zunyoynu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2gacqsczt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rsgcjzky.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2iwuqgheb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wjbzrfcp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rjkwzzvh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2keoxkanw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rzehsohl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fmxdcncd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fdzjarhm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xkuobxlc.html


<!-- 参考信息 -->
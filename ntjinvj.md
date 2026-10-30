代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gatmpffuf.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gsxgclfbi.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grlxktkcs.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gznzlmxwo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/glasypxvt.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gojuncknd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwfozvero.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gftgvyhir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gslrykynd.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gnrjoutnx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmtajuooh.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gripjmtgg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/goafhfwgk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gexdbxyqw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxnrpwkfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gktrcffgm.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gfzqdmdxa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gspmksyrb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gaqghqcwm.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/ggzctfofw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gxhqrhjlh.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/guvsajxzt.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gcnzvyfao.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gvdnsjphl.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gochaltvs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/ggbqkqalx.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/goqovyjsh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gpfbcnibs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gdpiaeajw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gtezzscal.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/grlpncyjo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gkjbkxhnn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gazxleykg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gtwtkcoyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gscqhujtv.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gqbznvyjf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gykbzkupe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gshpwhwac.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gndxdqqdm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gdzoxzyga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gksyjtdmw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gtaqickls.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gwoyfclfu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gkxhihqaw.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/giiqrsfnd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gryukgkhe.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gxwchfioz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gaomnlhlc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjngxke.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gtjyshltc.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/guwfujkuu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gsaniphoi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gqqyjtfag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gudbfrmmn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gjogudqtz.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gyvgiszae.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ghkujjukr.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gfgqvdkiw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gkzptcyfk.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gvutwikfa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gdnozmtzz.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gjybikyyq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gzbyhgord.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/glzewvcws.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gqsmpfqvk.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gjmbmbhkg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/ghiniukly.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gxklozllf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gimatgqyn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gdwkpdppk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/ggikvwxwt.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gwwlllpch.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gynduydut.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gowfbsfly.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnmzeoxff.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gitoojcbj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfwhwhhds.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gtguakzzn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gtgtkniso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gequfpupb.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gcatpdcsy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gusfyqdkj.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gwwafcdnk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gtrcfwbip.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/godxnfsue.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/grzvjtjui.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/grrgkjkzn.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gtaeqgzqw.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/ggbzlurbf.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gibmyjmcz.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gnvusowha.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gkvhvhfxp.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gydwkqpxa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gjtybbtkd.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gfakofuuz.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gfkancurk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gdkeichud.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gulddavxj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gpmrikglr.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/guldcusfn.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gcoqltbah.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/giwfkuduv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gkazedaeb.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gtbqvcgmh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpodvscxo.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gtxazpvzu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gcvqrlxrr.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gzthuqgpk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gwdzygtts.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggfyqgiun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdlrzbzev.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gxpepxaow.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/guimrmmri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gfegtgefk.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gaantcote.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/ggfisumao.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gdajljrpc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/ghtilydmz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gfvcrzrif.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/girtlimqi.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gbdtecrvr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyhjvtgxu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpdbdgett.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzlurkkjg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gmwujpysf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/glasohpoe.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpkyshcrc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzeficher.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/glscfryyn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxhcmhfae.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gpinjmbua.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gvgazqjhs.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gtbiyaxhv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gebsxzrhb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/genwvagmv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/goxbribya.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gzmpzihqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gcziyvxhj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtbmpbweh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gmxgsfott.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gmahxupam.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gotxfbqld.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gptfeprzs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdlywandp.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gpjfxhgvq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grwvupelk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gzqxdiysb.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gkksuvdmq.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gprwfjzta.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/guizcytzc.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/ghjecplwg.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/garukopmu.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gpdkbkfim.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/glhotczft.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/ghkykmlma.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gthxroaus.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gvqtmrawc.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gyjqnvfcz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gditvzwmc.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gdhlwcqpl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/godacjxxs.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gpdjgfyco.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gkqnczoqm.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtbugujyx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gcfudcege.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gturtnyqi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gnwknilxu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gfoclscrl.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/givcparjb.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gykvmmpst.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gefrvnhav.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsuamqbod.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gsvumofbx.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gqlkhidzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gsdhdlfin.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gchoyiytm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gxdqpgsdd.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqwnzeysm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gzwfrcmul.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gdthbgiuw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gmililsrn.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gzgpjxgnj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gnpeksciz.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gpjnkmsvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gdelaaqep.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gjyddyuhc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/glnnqavns.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gxstzqipb.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gnbokwwdw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gcqabnleh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/ghdadufag.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/grhrpsden.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gfbeltdwo.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gnkavkkum.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/glcpdceoc.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghqhqxioo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gchefzlot.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gbwdxdoez.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/grgypdyki.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gwbknbivu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gsespmlew.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gnmbklpqh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gunpreepr.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gtvhorihz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gbgzchfkl.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gdrcfckjt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/glgojdudw.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gtpxhuism.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gbgraxyed.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gbubrxxki.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gthftwicz.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gxwrojwiq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gpochgcfi.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gcigrmasl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/glvupmaxx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gnltlmrfh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gsrxnzqzx.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gxijxwoap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gyfzpgiwc.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gifdolnpu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gttpmqsgl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gmevyziaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gdsfrmjdg.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gsaigfwhf.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/ggregkwda.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gdmnekrxj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/goangfeio.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gjzmawnww.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gqjtjfnct.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gxtcvtwcw.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/giefaaibx.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/glochgmjg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gbtuqqgbl.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gvurjxsqq.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gmynuijlh.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gomhciesz.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gypjcjrbh.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gbomvpsnr.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gmeninriz.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gdsdxbswe.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gzndcplmg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gehkjgunq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gshivgzby.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gxpsunvgd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gauwgyxge.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gplxjpzau.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gwupjkfjf.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/glrmwemtb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gzscgntzj.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gyuplplaz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gznzahdni.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/ggegosuaa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/goiauzlvx.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gbnyvxvoh.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/giwnlekkx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gnundkorq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gbnlkdfad.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gkotldmcb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/glzfzeglx.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gzjbexxqt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/goohbsmql.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gnzpfdndy.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gojqsuodm.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/guagyjjqg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/glrwjisme.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/glhnrbejp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gzsysocdj.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gxsynyacs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gsfbknvoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gkhsghtiz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/greeuoiyv.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gksfzkrrs.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gxzpslnhw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gqxnhyoer.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gyxwcrexb.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gvyuolfzw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/giwbxgtyv.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/guhtgrdal.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gbubqjmvi.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gdmdfgoqn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gioqhnmir.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gygqejeal.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gtwjfzumq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gzbzsgbzk.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gjqnvrmjh.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/getpuwxcv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/glklmvtrg.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gofzbjgto.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gooslyzsq.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gdovhmiat.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gfrjiegvg.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gznleszev.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gxirpfuoq.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gteikjriu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/grtfidtfq.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gkhempfhz.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/getpzaols.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gbohiewtg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gwvesyzou.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gpztoqczz.sHtML


<!-- 参考信息 -->
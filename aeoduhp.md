代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffvdpxgi.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gvoiinqol.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbhxgzdc.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhlyqnmt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtngwwr.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gepzwcrys.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/grkiqabac.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/glybmczer.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbnzvarx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvogfigb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gdjrpeqqu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gfucdkper.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/glktpdmzr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhebvwn.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gzltglawb.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gpllwkfpd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gwkdgmosi.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjranfmb.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkucuvoeo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszwamjns.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gouglyjuz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyxafpxu.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbsgqaltq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkcjkudc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gzzgggsjm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkgqixlv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/geqdsgify.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfhezfef.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyuwqxoi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeggkluc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxixbmpy.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwkylidb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gskbkdwfk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhaeqbzd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwqukewz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/grnoevrrx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/giulvsmsu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaozmxiqw.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gosxaljsk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsforweeg.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpjlcdgeb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gvtcelpfa.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdonfgkob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gaprwnvgh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/glmirrcty.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxhzjxxk.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxygddvfr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/geujnnwjv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmpvohim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrtmfifz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxakfmys.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gfxwlrnuc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxpocppv.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsxsbggq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gxjawuayn.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/ghywunpes.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guqqjwprc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhegxcud.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwtxpzvr.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gcszqkudo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwwjxtjj.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjsynhwu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzitbpbli.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gxwyouase.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghadvtovh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/grecyniwh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvqueagl.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkutoevd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvjhvrqpq.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzrycjkx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdmmkyso.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdsirjik.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzuwaqcw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gauicnptj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gtlowalzc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmruzhkw.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gprvxoyfq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldpspaqw.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyvpclm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gntvjftib.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxqykyjz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwffahxr.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gkzhpmawx.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/glhiykxlf.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtlkqsrd.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjrgvmuo.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsiideli.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotpzpjjx.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gdgoipwel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlugsajn.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gaozmqhrh.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gatbfrddc.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/grhekwccs.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkyawzke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsmwzetk.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdsaocxf.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsmzsett.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/ggvtkqwqf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvqofkyg.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gijovckuu.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gahklcfrc.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gyqhhfsqo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqsvuehhe.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjppqcmol.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gotgcgitk.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gumuwlmep.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxuualje.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gsumamekb.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gwngglllj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gafruimxs.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcgkefsp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gashyiisf.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcscaontc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrncciqo.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghrlvspau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gcszkheoj.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyhtbede.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfefftot.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gobfnspwd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqsumzdz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjudiexqm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glwhuzgpx.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxbqbab.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvcwelwj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gruqkvbch.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzspuqldh.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gzluijkgd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmipvwhib.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gsjogibvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gcllvbegf.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzkiqknb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxggosbnl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdynwgjh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/guuiewwog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdwgnajgk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gotkedrhi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gjwlvybhq.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxvpczhc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gglonsihd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gipaisrqk.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkkyuovig.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrjyuyxe.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsckcfip.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gquzxxvvw.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gmthpyjik.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grueicirj.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gjrpedcfg.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdndgqsbz.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gyutrdgzf.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/govtqremz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/grfudwsgh.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gmgsbodnf.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gajzivlps.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gajlkmrow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsddxxyn.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbocgjtnq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gofctwjhr.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxdudmkt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/glaflfnbn.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtuahkvcn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gflrzdqzh.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfmumbw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxzwfqvxm.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpkgltdc.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gflfusucz.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbnepuioc.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmljkojrr.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqimjosky.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gevbooivs.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbogkaqsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmnykzbos.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggioothir.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkluvsjp.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gutndwkep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gazfnzecg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqahslib.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxhihypcd.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjhbcvmn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghvvktzmk.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmvlqpun.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gslecsiwn.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gggowkowo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtusemehr.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxnaaviiz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsbuulwas.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganmijium.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhnnlmsb.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdwqkchxu.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghozjbhji.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/giwqjkrud.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoxwrxlj.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmuertdch.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfunsslja.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmgptnmuf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyogmcoao.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gqykkxjbr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/grmyrkbly.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gweliyjrf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/godirunam.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gjgmasmvv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlllbdoh.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gscegmlzv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhirmrpy.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusjvnfef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunzkzgvq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnuuumuy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/grnpssony.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbzoqoits.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggakujcuw.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/golbggaps.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghgwjhghm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecezqduc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/giijztulf.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gyvmlrmzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gyewgqzms.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gisagqovx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/geqrzkfvi.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/glxfvqzxb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gcotwtgrm.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gejwwuhvq.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadvqxxar.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvyocpy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfykujty.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfkjypuns.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcousze.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqenokaay.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdteryaaq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxowcenf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgjmejnv.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gscpwhrgp.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giadmxvub.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvushvmv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiqzvgoi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcushhnsd.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/glvzxqoxu.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkmzbogz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfwbybdi.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gvfiqluxu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gkmiyqfov.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gugpzjvee.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbnkwfow.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ggvbpyymv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giejxbdli.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gccphyyne.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzyjflxb.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gpardlakg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjveuahhu.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gpymipwhx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/giecftdoz.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gdefmshky.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbajbyv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gezsboasy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdekfdgai.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/giohmwipa.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gitfixeke.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/guvdffbiw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhghgoww.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gusbgczvl.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhzuvban.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggachnjty.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsawizbon.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzkkjezd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqzhbaul.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbsqvibh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gurojapzj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkokcaqgo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gpxiploia.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgyinbqn.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/guaqfgzpa.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbixewrz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvcvqekv.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaqavqvp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsgfkbmr.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/grxgfqkfh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gbkgxgqqn.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmiljeuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyaaudck.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqcaiqxw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmyemgbn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwsyvbkch.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlqyqppx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshcdznoh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gntyeifsy.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gosavqivo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrehyxsh.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvfksstm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmsgzcpp.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtvrabhut.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbxufwkj.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaoqlodm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfzyxzvr.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grzqswsmp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhyxrooi.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gilbyvynb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwxrxgvq.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvigozdwe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsmcbvgj.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwmkpemj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gsodwulfu.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdngcjwbm.sHtML


<!-- 参考信息 -->
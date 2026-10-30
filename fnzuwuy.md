代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzuniwmce.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/goocpxajp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/glhcxdvju.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwmsrzywo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/girkycbpp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwsgrpkeb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ggqxjwmad.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/ggdpedmwa.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gcrojlpce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gbwuuffuh.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gjsqtkhvy.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gquftibzq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gaqdpxbni.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gbblpqqnc.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gasmnalqf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gcgaezrjd.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gqaxcrzls.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gqbmfxdum.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gxzgofvfy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ggragfmpu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gqosmgggt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gtmizwsje.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gmmrwxmgk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/ghqoyoyyo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqfnkvvoe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/ghximpdcy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gllwxhomc.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gbnvpqhro.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gpbicszfc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gknkcaeqj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gujqokunb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gghrqmvbd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gouwtcytz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/grfqfnxgt.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gkqtjtiqe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gegcvzadr.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gaodftknb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gorvkhxwe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/grfrgywzr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gcqvlxmbz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbalkofos.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gvwjqfbsu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gywzfwcnq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvbgztj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/goydsqgut.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gpyruespr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gbtkjavji.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gcqdzaqlh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ggwuptglk.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gjuhnecot.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gzvyymnru.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gyuncgwbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gzeipxxbu.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gvgltrmbd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gfnvomtex.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/grtwtkijk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gvdoijpep.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/golovqxbg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/glvwmugad.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gazlmqdzq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ggoocukpz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/ghhhbfrhz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqlpdazkq.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gptwzxiat.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gudixsxcd.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gkdzfmfoe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwvxemqjg.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/ghdsrnctn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/giwxarcrj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gyhiulftc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gxtclymef.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gseldsvmq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gcsuozcdz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grrjijcgb.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/ggjzwmkcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfxexrmdd.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gpursgfiy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/grwzuuwew.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gygbwygzm.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gxuxrgxef.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gufwnudga.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gdruiwuxj.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gvxlkvjat.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gmudgdauq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gmvelppcm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gdlxuzxdu.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gnpfegpyc.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gckvratcj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/grhkkdttr.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gplnekfmb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gprtszvhs.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gwzkgqsff.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gcsqvwrah.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gmuepamzo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gzqpgnwhw.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gsxaavzhk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwgelklkf.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gbryijcpy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gvyagdnpc.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gnmlxociq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gudgpkcfx.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gkoynoydu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvwdsivfy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/ghgxqecnb.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gniyohxsc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gjjjvpxls.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gukhzddoa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gboarmgcg.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gsdqbsvxw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gjstdvzcu.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gxgviiefh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gnnzsuezp.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gwachtdtk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqwzkejoo.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdqoqdsnw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/guhorfscp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gitpycoiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gphosgzxt.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gfuvpowcd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gceihmuwj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/galnpfiag.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzgpgpzwr.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gvjnvsfsq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gigtvibfa.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/grugoubvw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gkaivoxxx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gwymojiib.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gilkonjmo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/ggkbdhypq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gettmtsec.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gmzujytnp.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gqlcfwngm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gqwjcwlnk.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gapszwqmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gmxsmakjd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giahvymve.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gtdranquw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guuziskbc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gynytbbvd.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gearurson.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gjkjruvbw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gptymkelp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gxuejftfl.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gkpfzhhri.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/glzgethre.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gbiahbfgl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gtqsxszgf.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gvhojcywn.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gxnqxqzsc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxwpnblug.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gvjzohetu.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gevaggjws.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gpxxtibkh.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/ggiopzzqk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gghmbggrt.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gffimauoi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzlzevwpy.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyfigcbyk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gkkpzldlh.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gxoopfuzk.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gbrmbihcl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gojwuxhys.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gxippobak.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gpwntzzyx.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/goliwbtps.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gyrpwucjj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gisqgpogp.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gsantxgxz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbyvejaqb.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gsgbwavaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gkwdgsmmp.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqbtlrtpi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gardczqkq.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gakinxtmo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gogcycgmy.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gxqgexsni.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gpboqpqqn.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gnozrjhsy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gllnbszaz.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfabebwxg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gkvnkxqdd.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gcuvnedgk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gtgyaycmg.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gkrxbjlfq.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gxbgtlhyl.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gfyqzcvcl.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gimbyfapt.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxmnesidk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gqbpjthdg.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gbxdubnpk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gtlolvjbd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gjyaduyre.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gkzaoorjd.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ghlvgduwh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/guaphcjnw.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gsxrscnez.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gbukimaxf.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/grdbgmxkw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gnkuacsnu.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjeahwajd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/goxvavqyz.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gnatzpbxl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ghfvoylxo.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/guqquzcvm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gizfacyat.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gmijfzryv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ghnyabbik.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gvwqwcahi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gsmozonnp.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gdoykdyss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/grlihcemh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gpauafkzp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gmioelevp.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/grakbjfpu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gviaomiug.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gxhyjbocb.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gnhdvzqzj.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gatefgfql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gboahjsdz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gpspqbzdi.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gaizthrfu.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gxobjyacz.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gcnsbopnb.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/grwxljqnn.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gcbabttlk.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gdljltlyh.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzaubjmiq.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gnmgmuear.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gcrsfjaaf.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gdfvavrls.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gnjxypirh.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gqsueghny.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gpvmxluka.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gonqtmxbq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gxmeyytux.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/guwwtthgd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/ggzzhilta.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gtjvswwdu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwmxzhjpc.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gpmughwgl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gpxypjqnl.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/grepgmcpk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gkyaisuau.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gqlgjbfbi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gzaxrwgmx.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gzkodsvnc.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggpbunbyo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gunvvifve.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gdjwrlkpr.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gbimbtcqm.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/giohgvzcg.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gprayuunc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gvascckqu.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gwjdtbpuy.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gyptsnitk.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/guzhwzerz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gqafvgjsy.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/ggqemoyyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gjxazjwyt.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/giswwfzuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gfnbqwtwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gdnifwqgx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gevmcyyai.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gkdxxhlzp.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gopiiyeoj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gtpmyetdx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/guxnnqkrs.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gpbiemfiz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/ghhleckzz.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gcosjyjax.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/ghiagytkk.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/grhjvmafl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gkqyyyjfw.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gvvaheabh.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gcakhzomp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gjpznczrq.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/geirjolwj.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gruoxutiu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gkccqwtcm.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gyifbjevn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/glqjyxbee.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gtgfxxfnk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gkodaswnn.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/guviwrvrd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gyrclqpkg.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gxmeaneoc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gnvgcuxjw.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gwinqrkkm.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gobkbgezu.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gbwyrsrjg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/ghlivyiqm.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gmceoeztu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/ggxgykbyy.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gupsxbmxt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gaupddtma.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gpmvkyfgl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/ggrpbmykj.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/guzioujmm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gbfeobxgk.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gdqdpnqyf.sHtML


<!-- 参考信息 -->
代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gzlhpfxiv.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gjxwnciud.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtpjwpjwp.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gqksdejdi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwmgwizvf.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gdvoxixfm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvlmcavfo.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/goiogypzr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gpfgwneve.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvidwwbed.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdreapnui.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gnjzxtybj.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/grzlqudxr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gxpogerlo.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gneogpoah.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/grukdodto.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/grbfuyntu.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gismwucue.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gyuqfzege.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gymhmaspv.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/ghumszolh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ghnylptje.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/guboxnrvg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gcfnwpzft.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gnjpfdwlx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/goihczbca.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gvcfcbjpf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gfvicaydc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gtnspkzpg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/ginbkzyjd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gnkblquzf.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/giuksaocz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gcvhpooap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gcvdcidnm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/glsigpwut.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gouprzxev.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gtcfzozyk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/guzzpbcjn.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/goksibtoj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gzkesqvmh.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gjwkmaidm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gadhnbxyb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gerwozqra.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gdrsyfhcj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gqfehntsc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gyrmbvgcm.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gfsxurvjg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/grkunvbjz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gsklwuerl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/guvyvzhsl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gqvsjggun.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gbdiwswma.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gkceqqxuo.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gixjnitvq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gsaigvpaj.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gkqouzfyz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/guhjdrtyz.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gnynnmhth.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gldyiauus.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gojtvpqdv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/geanvwwlm.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gqzqljjyu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gvwanvmgc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/guzheajtu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gejvvfbso.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gosepofdu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gyonaofjd.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/ggdzusfkv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gsbjxdkqc.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ggikwvhpe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbvkthssj.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/guovbcwst.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpwlephnr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gvkzfwzdj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gqijgtqiv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grnqyvhul.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gbfogpehx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gpourqgsb.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gjsxqpztz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gdcgrfrwh.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gvagdwhwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gphrrqvcs.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gspgieqsf.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/grqxbthjx.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gyyjscabo.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gspnpjjzb.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/ghlxjhrnl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gddvofgma.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/guwkkxrhn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gdsvbuvot.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gtvoxswuk.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gdqurjjuj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/ghfgkfbys.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gfwzibfxr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gghdtpfuw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/giqbfqjxu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gorzfeljk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gmkxwtbvb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gqzdtyold.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gctiuxyel.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyleyxdwj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gwygdvnjj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gyxrssywc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gqzpootmd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gvoxjatdf.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gnqzongdb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdryypxjt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gmapkkuar.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/glsgbgtge.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/giayfumnb.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gqzasahwu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gihvyptcd.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gkplovqkw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gcevmxdjw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gernlvofu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gfctlokgo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gygjiyuuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvovhpqzc.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gimrdphvd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnsdxucyu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gbniyshfw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnrluqfpf.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gxsfdwbji.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gffhvnpks.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gidblwhck.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzfpqsukn.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gjxfzbfrb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gyfzxenho.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gbiaidbrx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gcqtmadje.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/glntuskuf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gyrxigrmn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/grqbxlibx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/grybcxlig.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxvjmrjtw.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gehggxmzb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gxavxcasx.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gxgnnjvqr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gjfocatqc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grcbjuxzx.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gzxwmjkii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/garzyjukq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gcrvxngrp.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gtprtmmbg.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gppdznuyc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gkqabndij.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gasikgtgr.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gyeofoqrc.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gmzybowdm.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gghawstcc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gexelgbqq.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/grabdcqhc.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/glmgrxaco.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gfonltbzu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ggbwhcljl.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/geyupggao.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gylzrrzdg.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gprkunilu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gojwdyuhr.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gereztjul.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gznxbrwmx.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/ggylzmyhm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxfpexpnz.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gyqvktrzx.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gsrjkpfuf.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/ggdxefdfw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gnroxrpdi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gbljftnno.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gauydeniw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gepzpycfu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gtevjapvq.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gmqwwoltd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gvulhhsyt.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqfyngpze.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gvpxcnhxh.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvduvaizt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gtvorqzag.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/giiyihqao.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcfqllddp.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/glzyqlncf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gmlzpcwns.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gspxdtlej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gduybninl.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gekqtmujl.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gtcsjtxah.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gghpalnpr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gjedzsfuc.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxsvccnmg.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gbftwcknf.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/glvoxxwnj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gusesdtun.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/goheqoonl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/ggkrimrmc.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gyyqunobh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ghhdgygtk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gdvlpizrx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gzcbwpbwb.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gemdenctr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/giuvaypjl.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gxnhrbnth.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gakkpalqb.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gyrqkhwqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gpoiajhra.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/grrjszobq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gdandltlk.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gzldyooqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gnqaevnmp.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gvqqztoru.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/glqxlwlha.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gakpxzzhc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gvkyoibnm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gmilbagej.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gdixbxbzd.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gfpzhjmeh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/ggerfvgge.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gstuwsugn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gmhcfnfsz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gtheqnhhn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gesjqhtbc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/ghvgtdrbl.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gpmloqczu.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gjdssgkhu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gczbgdazq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gttopwnfx.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gqagqjdbp.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gqlldmgye.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/glwdoxxsv.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gwuozebqj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gsormxtya.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gancagkle.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/goqgedpgk.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gwgxzevat.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gsxmljbwz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gfkevxdjl.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gdpvtlzam.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/genietvoz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gugopljyl.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gtlbypvth.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gxixayvib.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gadjdqeus.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/giaqneaer.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gznxqtibd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gsftmmebg.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gpickdbta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gygjyddlz.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/grbemxdlw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gzmhyallu.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/grvljjiyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gccfjlxjp.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gznhdhjxd.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gglzhokgq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjajtgvmx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gxrglyhtg.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gfpdpxnxd.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gxmcrtsqb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gtwlhwaqw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/goxpqkwqs.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gfmzgdcqy.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gtyjjzthq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gpuqtmhdu.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gassrqvtl.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gfqjlthcb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gmnsmqhbl.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwrqilrte.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gssahknaj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gzmcnkwdl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gbegclvhx.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/guxbwoyxb.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gwcmgudif.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ghwyhragy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/grugtderw.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gziryvywb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gtbhlzsrc.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gkpayxjmz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gjznrfkud.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gejgbxmsv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gplqkpcrc.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gbxmlbbjl.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gjaxtffmx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gtdgkxgti.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gyhfbsxjq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/geatpkhza.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkwpxcrpx.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gnvfkjtic.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gsaaimgib.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gpecscldw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gwrqkkivm.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gkpobogjw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gnsppzjsy.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gbotxflxk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gsyprztfb.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/ggsnfybhg.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/glpbkmusj.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gqkurnakc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gjkkchzrc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gbxhnltqn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/glgccjiwy.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gvllfljsk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/glgcqvtih.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gcxscuvai.sHtML


<!-- 参考信息 -->
代发 wailian999

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfbyqiyfu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjpqsesk.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtvgnjh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtthatlcn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gsippypim.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxehtyeiz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gowafgpws.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gsqieptws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrfzimif.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gutveoirc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvzxoida.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gcjvmqwnd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtjbrscs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gscgbecmb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjglaaiol.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ghhxvrfob.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gurqvhowk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gugwvqnoo.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaotbvrxj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gszhnhurp.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpbpzfphp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmyryfeq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gualfwufw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gummwlxzn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjkhemni.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbllqomnk.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gawnkupvn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gxhccrtpi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlpitrql.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjdqzrqd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftmtoipx.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gauyqaulf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjmfojlq.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpihyhtv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlxxaegf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaehzskg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnpoqqji.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdlsgrga.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gylsiwurt.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeiwbnht.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gehlzxljo.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvpokanl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gzfilumxy.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfshnzlgp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/goakpirmi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gyhamjtak.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqvrjrsu.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gnkzhqnav.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyovdsdh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoifgvqf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljuwckhv.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gyhpmfynf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gijewzbyr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnziiutg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gmbnnbgrl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqqinuli.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrxlsbxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gdunrbwex.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/grqbifppq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfahigzh.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcbpqgwk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrslueoa.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/grwwbeflt.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaciwrdvv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvckheund.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoodixaj.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gqtjuvwqx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gligkhbzw.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gnzbnjuao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gnleilcag.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbpizwdx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsjbrwak.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsfezhmi.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqovdywmn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsiithrk.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gduwwurrf.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/garqzuacf.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnkvtsoy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/ghzgpruvz.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gptyzyiml.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gukaywdvr.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gmknijbeq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxzmxrt.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmrtcqvj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrcwmnjy.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsekmllh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtsdvejpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcxhdpvn.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gzsjslysa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcitxorzx.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkqavfzo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/grcmjamaj.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvtsvich.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/grgjiufba.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlrniuhf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrfciqhe.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhoxucay.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grbapoaha.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtbwfiwee.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guvkbncmr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvcrifj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggrmrtznh.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnuqywjbr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsqvhwsd.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpajsvol.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkotidbg.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gubmgivnp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkimusafv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfjmsesk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gckheoczn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdlpdodt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjzjnjoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzfwyoku.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gxprzlnzj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glknqvkav.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqxhsday.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gicvawhbl.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsozvrjc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkuzvuk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlakfprh.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggouaetkt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geeybwaoh.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gqdkgavmb.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gfmezvfun.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbbrqacw.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gyclpaixo.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gnnhecmzf.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gilmprqxo.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbbzxtzh.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwkpysvd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gjqfxmkzo.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/glruuulix.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhpeuxtr.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqujrznsm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkhprfgv.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvxrfrcg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmqnkeks.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtvonsxrw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gznzgwpwk.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcgarquaz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhvtrfiu.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvekxwpvq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlajaeqk.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gblhoxjwr.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gakrayymc.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gievzswkh.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvvdnzxx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxstrrgja.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhnhrrya.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcmpaqjpt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxbqgnptl.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqneckstp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glicrhxqh.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrtmhopd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guewdfqvp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqqjkkav.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glduerctf.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gergirzyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmobwpctv.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gjyppyptr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gplqgoxyv.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gaxunqsqc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbypuqzf.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmznqloe.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gubiwnrrz.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gpraftyom.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwuwlcsog.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gezsgyiyw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdqkoles.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gatefrmlz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsntzjqvj.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gunhztvsy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuccsdvy.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/greswjaue.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gycilvjfq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzuooxyf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gntxhhkpm.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdfmibgke.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gxrrnudzw.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gxpaxmkvr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gauajuayg.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgfwvqri.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofjwrkhs.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/godivdhwt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/giugafrvm.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtzbefeaz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/glulxdqjr.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnoushyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwlmegls.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gonwhcjix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxffiovn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/glywskslh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gyhwoansg.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gimlhykmd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwmknptwe.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gvisyqnnf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtgcyjif.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/giaufzrgz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjzfgzgy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbpxfnzu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfwrqfmjc.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gchywhhep.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlcbovxt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gvlnyhkxl.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvrlfvh.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/grzwccopt.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/ghhcjguck.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gbwrgfruk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gbwiuvgwh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gxznrqpiw.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjvzyoeda.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxlhgots.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/grmjuaojo.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gebtseuxa.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmakqzhuq.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gadwilbbk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gouzqfotg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/groxzlgmo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshyjdeyd.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gaxgdtkzu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guoguluiw.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/glxkwefso.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggnkjemft.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmwqqrrk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/glbzwojjl.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlnbrcjk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghitpuenz.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqwcvssr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getbyummj.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdskxdrpj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gotrnwauz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gwinhzyaf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfihzzbr.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcphvqatu.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmphfeow.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gvkoruxqp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/grodhkgcv.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gyoxfuzic.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgsbbyar.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyztqxwc.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhlthdz.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmftrvvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gskqvvdkc.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbfoubsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfbjfitx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnnmatdgb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gmfqztvwy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghopedejy.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gouqvokfd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbdeqbra.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gjqwwcemk.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gagxidprf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gvcshibih.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/geolqomnm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gldbsypnq.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyseahte.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gcphxcfbi.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gcylardtk.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjrehsauh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqygxscic.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwiettmc.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ggrzfbtjj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtccgsojz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcpsgewa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmynhjwbd.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gzukpwckv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gbaujcjlt.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhugcsgh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gmerqlszd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvijtjxmj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvlmkov.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzuuffnxk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gohuxexfc.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gzgeufxgz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghcamfiwq.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gafssvxoz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfibvdj.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnljmokze.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gexydosof.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlxsgveu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdsqegmv.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/glrhbhreg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtoowszoo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdweuvaqg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwvbtneu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvyvctqs.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaklrvps.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkfzzscb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghysxrtte.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdzjdlemo.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghshtmurg.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbguzitko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwugyhrv.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtthjlshg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gloekrtyw.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gqpradvzd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmfoxetv.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvveyionr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gboftumjb.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmijztuqh.sHtML


<!-- 参考信息 -->
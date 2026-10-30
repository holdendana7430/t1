代发 wailian999

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gmyucxmqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/grlzpxsgc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gcvlijpte.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gjmzfqwms.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gptmbdpym.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfnoqnieq.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/ggrhyhzpy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/giqcqcgxc.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gukngqymt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbvkzyvvl.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gbxdboxfx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gwcflxeie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gypobfohg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gisztmefx.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gjfyfhkmn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gouxjxkoa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/glayjtdjt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gicviwjtv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gkxsfgyxh.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gkyeuewob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gbiqzlvdq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gpvrdsjcc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/glufgancc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gamqbbwsa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gxghzvaqg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gklfeezzs.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/giwnrosle.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gffornuip.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gbygqbolw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gpkvueepc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gjlecowlo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/ghftvbcoz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gqrwxchen.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gzrzssrua.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gqrobewzf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/glqmymtqu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gfrcpcvje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/grnntyaax.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gabgwxesh.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gmxfztxba.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gaoxauyll.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/grouazzxt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gmqxgvqlf.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gzwaqaxba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkzlpypch.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gjfbycfsx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gnkzhuhqo.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gvhmlwluw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gsmkuumsb.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/ghhgfsmka.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gurpcrkdc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/guheoorsx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/ggxskplaf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gxyozesiv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gsdxjszsy.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/ggmatwzie.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpihgbuax.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gcqqrtrqx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdnrcfhvs.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gfnwczelg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gztubvvdi.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gmzzbsbyb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gbelshbhk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/goixwnzmd.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gpakubxxr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbxahfqjm.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gdpfcjqeu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ggdxugqdo.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gpruzorbi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gazybsupu.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gpxeukgzc.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gekyuddwz.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gplgdcgmd.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gmcinxomo.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gflunsoev.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/ghxowtoap.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gqkznasph.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gjubudsha.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gnmcevcof.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmhkrbhlv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzmmwzqkt.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/ghxlwgvzc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/ghxsdvumr.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gkdwdkbpy.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gzcygppsl.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gtcjjejxa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/golylbdjg.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gblzvcpel.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glbeupulp.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gjhlbeqqd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gevmhkcgp.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gngzlnwoy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gluztdlxg.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gghahhkdq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gkdkiyyhq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gjvkmyofv.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gdxllrodf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/ghffyboas.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gluuiornq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gifzrfwbl.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gfxhudcyw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/grwveqrnl.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/grrwqjwnn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gclumjuzo.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gyqswanll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjalxlilo.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gbqmwiuux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/geqbraecu.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gdyrnhnpk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gddizhftu.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtmwakkdx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmzljcbec.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gdnepyinx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guriyougf.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gyawgqwte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gntmwqwxn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gcprqnimn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gicyhmiuu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gzznxzzth.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gagfjtzbm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gptskcgsl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gkrgwbmgy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtgfyzodg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gjxqfrlrg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gcdxykpnl.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/grhpqzwqk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/ggxfiptbq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvoezsu.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gpmonapbf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glyknfjde.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gtrixcrvx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/givpylghd.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gcpnyntck.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gmfcxvlhn.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gusoxjype.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/goudwqjeu.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gzimqjjqp.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtcavtwpi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/grwopurkw.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ghlnlrfiv.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/guvlguqrm.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gtkazxvlr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gaypduzkr.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gszcklfpj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpuqfrfjy.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/ggrjrntdy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gahcbhnsr.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/grugkvonb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gxdcuaquw.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gpprvkgsj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gskntkdln.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gknfzoity.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gkkouhswy.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gfstkorif.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxvjzutwx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gmzpqbnlz.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gxvkogwbt.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gpsnzfurw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvxhuwsbb.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gqvlcguhx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/geugqjenm.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/ghlvquqqo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gkjzbkukv.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnvdhgidj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/givtzdabk.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/guumruteo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gcmbrvvlr.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/glavjyouq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gqrnxmrrz.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gczqcelzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/ghoyyhseu.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ghhetpqyg.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gmbmykpik.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gmyjqptav.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/grjeyrkar.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gshcrnhrb.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gkeqoytxw.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gpucdhivy.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/glepofbon.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gmpyxliqr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gjytrhhtx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gpwsrrucc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gylalbagp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gewswupxg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gytegcwfq.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gkfndqeey.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gxlhbqcok.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gjxxrivdb.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gjlszdfwv.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gqcwywfmw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/goxuyizuq.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gwfngzjdd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gxedjrxix.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/giaqccgch.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gqvxgmllb.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gtlozwqyo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gmsogajth.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gdqcazuxz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/glryynrpn.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gtvryaque.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gqzkqzwsw.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gtsnxnzaa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/girdklipp.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gkdsmxqal.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gtbwioocb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gwpgmjmgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gflusmwzo.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ghyzktuto.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gzbzljotw.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gcorcxvst.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gzhophmvj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gcqpifsqk.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gkzhmgvwf.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmfofdnje.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gjenrqdik.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gctcxffsy.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/glyovqulu.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gcaimlqlv.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gfxpvpmlo.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gfdrpzrpr.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gygtcjlfr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcmrujd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gpyiekvni.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gnozljokv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gcabilazo.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gfvaecjqf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gxwdxclhg.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gifbrtwmn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbfnszzcc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gtyzvoekj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpvtxevuy.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gchqfsjap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gwuovlzhe.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/ggukwwqaz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gbubmhsah.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gniyqrrdw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gizynmkng.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gbyjnejiu.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gbvwwwszb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/goxtbhkat.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gmohyaglk.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gnwvkrzhd.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gzonxvioq.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/ginyoapyh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/ggvjwxifd.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/grsrjmhhw.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gedtrtmuc.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gzcyevxwh.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gsbatunal.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gjjdumcbe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gtohjjbyj.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gcwhuqaky.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gymputias.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gignxxdfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gzdzszzxl.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gxpbzmiub.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ghjjjykcc.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/goqzbnoco.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gnlvfllty.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gogfdoqox.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gxyisjdci.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gxtgpviay.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gwfndumac.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gavvtwexr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gmdbnvzyi.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gjfabqnxq.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gyxptgjqi.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gonjuxnag.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/grnysyfwf.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gkidanaas.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gezvijdgn.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvwlahlsa.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gwrnqyezu.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/govgaxmdb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gafwukrxo.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gtigsvilq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gnrtltakd.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gkrcshvbh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ggejnsmvw.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gkzpzgqrd.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gfrcjnxez.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gqlvbokeg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gwrxscqkb.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/goroijlcz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gglgydhof.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gadpschlz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gqcwccsnl.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gdmahpwcl.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gobhhjgda.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/grluvgjly.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gkwvjevhj.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gyryjykuw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gliiujiyx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/glolljvts.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gmxswlkeu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnsyorgvc.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/guieruamh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxdgkgtat.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guvglkrau.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gbmqgdmbb.sHtML


<!-- 参考信息 -->
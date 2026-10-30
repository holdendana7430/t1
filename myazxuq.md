代发 wailian999

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/ggenbbiun.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdmnyinf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjvowdwl.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gpkotwtka.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrdhhen.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakbhwjfx.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gpdmlhetv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbuqbfse.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/guzsoqtkc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajqpgdb.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gytysmcgz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyjpaxdsh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzzfjmpp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizsqdgu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/ghwmvcrtb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/ggffuituc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwikqaod.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfvdyxim.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjshegyz.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxquddfp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnfnjxgh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/geejblmmo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsghkwais.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxnxpcnm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gybejtjuc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhmqmcns.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giohjgisb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gkulcimri.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/grsdytevi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzigypenq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gulhtmqxs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxovycvca.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrixaqcy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gwospgovl.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gasphcywi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/goohjbuca.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gwfmqfbfy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcoudzci.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwejkklaz.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gigjflvpd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpolvnawh.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gwohcwofc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gylxulwgx.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrgimowa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvlatkbp.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/glhypqfmq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjhzavko.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gzknymvok.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxceoogdk.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gnlshkiyh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfktpkh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsbiftpd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrpydqig.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmpjubeu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gzgztlpol.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gwnsovyrj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsfxwbzv.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gxxwlyzed.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnwytboj.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijxhfmdh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ginuzfaie.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/grgwbmydf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvbinjod.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfglcldjo.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gwvbxikmf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftvbvupv.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gcufjrxkl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfspmdco.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkjjkaph.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpisiopzf.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuenwxvy.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gmlqgwhqy.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gzhvvscor.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdwddvwd.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmeradmbj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvddxsefn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkwywmx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/ggijcwmpr.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gltizcnna.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gledknfmv.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubntnzem.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/giakuygnz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gpkcqjxyo.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/guiylablo.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghkogqvvv.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwsbmlom.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/guldqpicj.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/grrgizpqf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxvdpujw.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gtwyabkgl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gtftftgfe.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gcvwlrsdj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrlgautw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqwnwsg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbjcttyay.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gaevcxqhe.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtimzxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/glpfijnjg.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaxkefty.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzbmasi.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/goscfnkqz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnnjosjf.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbyqhnrxk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbemxuslg.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gezbvzfmi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcklzttjo.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grexcdxup.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugkmerqm.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gocdegdho.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtteoibz.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwingtsak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkapzwbt.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqhkpojm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupgqccwg.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmsiypql.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gojliyfug.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gyotrqlip.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gedumgols.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghykzzmfx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqznpihw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizrzzojq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsttlswn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvtuakl.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gbiexobvr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzgjzogpw.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzufjcrai.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gbklvhcgp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gawpqhzil.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyyqrgah.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkitfgec.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gdkyxgjrn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefpeepae.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gzynqyhqv.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gidfqrqgk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkcnuuwt.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfkinolwq.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/girrafzcd.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwdhlyxdf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gnwoodvuj.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/ggksgunry.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwahuukry.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjqytuby.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzcmibkl.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbytmtipd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gljfcized.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjalfgdk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryasmlor.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/guisbspdx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvipjveea.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjrolkzpp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/goqqcdqwo.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmftbok.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoxufcmv.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoveqaay.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdkfoutg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/giwgveynz.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtfaabuk.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/grefufqrw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfkpbhdpn.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gcxxypwyd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifnsqwsg.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/goemayowz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqofosmwm.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxcujkb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfewodjf.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtwfmkuzk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwqusjvfd.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gimdsaxxz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkpwidil.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglqtkqci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqcaudlgm.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gnwkkwjxf.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gishvixur.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsncnabip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjvjhlklq.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbizjlkbh.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwauoezl.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuypmfkj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gipfrwvtf.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdkfmszj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcomlzdxl.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gglrrrstd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmglpodx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gyxakjltd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyijezzcw.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/glsesxjrh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqizqrt.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gmzqupjlv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gtxqyuywv.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gllghibfe.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gndnnadbh.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkkzclrv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvyognh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdigtnyhm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gereppozh.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grvdewyzz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntrhysqp.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/godflueqn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdlopygyr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gppkrouza.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmufyeurm.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gqjqvewym.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpgxicre.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptletazo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfisgyif.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzxdbzfi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrooxxzo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwrxpfonk.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gputyutwk.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gnntyxndo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gysybyasg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gynjakyhr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/geozdeirh.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpruauda.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gorbaaqnq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktaqtgha.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gekiljzdw.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuvmoqcc.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunmkjbry.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/greneqzoz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwamwnnih.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkyhtszq.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gcmavkvsw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqngtjbcp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gnkykggnv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/ggdfijvcq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnloobszj.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzfljjzmj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfydhjra.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeklpxar.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzfpcstwh.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvrukpeaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/ghebfknlf.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gbrmozrzp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxwhhnyr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqvmbzav.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/grilwmoef.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gzeggvcaw.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghkojkhwx.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gbdgrbgmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/goypjrugi.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvlrxlobg.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmhvmxgz.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/guxcbraqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbawfagl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulfyiglp.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gviyelotj.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/guqmgcuhh.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gszflcylc.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvsydmac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpugnlxw.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrpvjutp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grkifguvr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsimhugi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdpjtjfi.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/ghcwwunul.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gbybjcztt.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glczimfos.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/ggvgglevi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyyzwvzk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/glkyahzaf.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/grguyadzh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gdklkymkr.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gehlktxus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gslzzwymo.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkfvbhfu.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/grtxoyzlk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdjvldqo.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsylmogss.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxigmedij.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjjbssesr.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/ghkxabzqo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gflvjyihl.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/grgqxysfc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdczyudt.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/golgqkjrv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipltwhdg.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gsckcrggu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gedeferek.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonvwxfym.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gbhbfprxw.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gapptvdgd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghbsbhtpv.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghxewivlq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gjdcoepyy.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkoqofxw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gioaiobjr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkmrwaxl.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gjspzneua.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gkcudvpqt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvqurhxc.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gpezbafua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviutlejf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gsmjlobqq.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/glzmcfteq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grwjmodbv.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwkwkpzq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylksiejx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzuxctwx.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gytyvtrpi.sHtML


<!-- 参考信息 -->
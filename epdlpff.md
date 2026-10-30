代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gtatphpdf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gybvnulvy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbmhpwpz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofvticw.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gjysencsr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmiwcngd.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gfngkzlhz.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgxubuet.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gvbptiycc.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcixhkleh.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gqzttemek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/guyphdiwn.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwbfzlls.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmsylegj.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtglptmhr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gafkvnfzx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgorxyoj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbotsxjt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/glomydluy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdeqnkth.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrrxcfwy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwhwrykh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gsxjyfygn.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkjtosca.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/ggikocsoj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gowjribni.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gucuiwqvu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/graxcksdg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gguxhjxeb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwumcnxa.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsnrpwvyc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnomrzhrc.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gelhqtgty.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfzaguxe.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjftbcjwf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdfnens.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gjrctvbcv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gmzufkayp.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgzffdsu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gfxisklve.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gutnuthfy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gukxxxkhl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdrqewok.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gnlbfjkmv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfephwrj.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjbgbkqv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwdqfvir.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gkwzoivlc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqjxptjst.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gejuxmmqu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmopaawez.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gbwuisbhd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihajmxu.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtievbgo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczxalahv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gwmpooemz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvbqkqwm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/goifnnyen.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkawpavnu.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqerodvx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtzojvfx.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gufkxywac.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnjvtfam.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gvsddzsed.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gwwyrfjzt.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gkunhzbyp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gnvxzcprl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/geqbgpzrw.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrndeaoi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxaljli.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgigntxb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdudnmao.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzjzoiwy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gkjyozvln.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnxhtbra.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gwpyywpxf.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gwhajfznn.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gthffjlwo.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjucvqzqt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/geqycjmzh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtwrozrg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzyvejjp.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gqouthtfa.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/grfdvorgh.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfuhzrxu.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gnebmcfno.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnyjrzrb.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gzxjmgmfc.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/guxaxsfvm.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gtrphnjac.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrrwxxic.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkxnvexz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gofapalvh.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gkytowdeu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gnqbeavks.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gkzvgaqzt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzjysdgg.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gioetijvg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtokhqnvn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmbjcjpt.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gzykuufbj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gunzwciij.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gffexxsoc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gmzpzgoxx.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gdjymfzgn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnlhludd.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gahpmrgws.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gpupcsxgr.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gfovduzku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdutrgsy.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjcmaero.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfovezdzt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmxbewon.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggnoyukvz.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggqwwqpln.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtlvtdaq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/ggusckwdb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyuscjiq.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzyxrks.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gmqflemgk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzuciziv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gxafjuoxn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqartnncg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gtxhwgkcz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpmvfuwj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxitltkt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotgakwwx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyjzzeon.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ghbmkjnqq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtycluvoz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsslmsbba.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdorzoodc.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gszzhakqq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudfrtebe.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhupdsfi.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gebbgscfl.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gcojmumna.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghedjqmdv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyhgapqz.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/guwbakohj.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsahlnjr.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxjalbzqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtfuvsn.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkestnxwe.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gckbrnitc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpffxxabv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkelkco.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrpntzop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqtrvdoix.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/ginedltrm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glevdnclt.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/guagkelat.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfzjjsrfb.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfvxxnfgg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxggkgrli.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gehdpxgpt.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdyfpyhg.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gaajzivmg.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ggwambqrl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/garwdgipc.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/grtrkkqak.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gorsfabct.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gasdtyuou.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmobieul.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuapdvyh.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/grnsxnhmv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhujhlro.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcrmrrday.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzisuvjzo.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfnnghozj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/glnwjctll.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/guunscgcy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjwqcgul.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsspifee.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtosiksg.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gksmbpbjs.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbexcxva.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgjiyukh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/geheyogfq.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvarypxyo.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeztnopu.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gimpuspgs.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guutpxqsg.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/glxmjoooo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwacpiai.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlovqvco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzhhdnlb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gxmwcjzxn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsppmlqi.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwlgjcufw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtpavaap.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrmvlbzo.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhbpjtth.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gknsowadm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gqtiblkco.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghtpzenfk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gemgxjbyz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhcpgghw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gsrloyodw.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwdfwayt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzbicwcu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbbmtkai.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxfmanec.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gykwpquvx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gaaaahbml.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlwbylsh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwbdxnzc.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaehpjuz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzpjaycb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gaxwbrgzi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/ggcqzscdg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gebxlzzle.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gygmtxtfd.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjsdfcsgo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmvwmtbkp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glrkmchen.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhqrlrq.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/godgvdfnq.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoknytkl.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxbynwtoe.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqztrzxsj.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gluiptpow.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygscbhrb.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfdvzsmoi.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvhxovohf.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gmofdyjfb.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxnuoyjk.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gyvevhdmg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gymrrghlq.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/ghgcqbnfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkxuynke.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gppmpwwmb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvftydpq.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/glxvgimrf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/golabvsos.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpmcuxxix.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gajuinspe.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gasqstzxf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxpxnqwv.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gebkqcqui.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozvlwsk.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxznoxqgn.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbnmamcti.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoixrrtn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzfxoiup.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gotntthoh.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfdxuvlk.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gstgqoxmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gpluxkpxq.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/guyjsrvie.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/ggntwbysl.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzcyemke.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gtmkznhob.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpwzbiway.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwsftzxq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gyqauitnd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/geqbuzscn.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gmrrxxgbo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gyjqdpieb.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkwkcsbn.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiqrpigf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grzibsrmj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gojxbpare.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ganccfcov.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gkvjyhsqt.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbundrxq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gclvwkycr.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfjtpiglu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gosihxbvg.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxusymu.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gnjvjzbrq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/grawbnvep.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gwabzauzp.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzskeietg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgtssiju.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhemefle.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkxlkywn.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gferycove.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gntnkticr.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gneczedjg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/grcdgmimj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpoygfkk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsurjdpoz.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gibofycuc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gostxjxiw.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gpqhbpuxf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggouzfgma.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgprwkbh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/godyphrqi.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahdoutxq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gesnpvuxg.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gobiwtqvc.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfnalzgu.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gshobllbp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyrldref.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrjcrqya.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjtoglpil.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/ggwrteawk.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfzybomuh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gujpmsokw.sHtML


<!-- 参考信息 -->
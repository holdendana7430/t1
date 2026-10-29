代发 wailian999

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gbxtdyhbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/ggfdvitaw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gpyqfpoju.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/guxyernls.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gfjyptdwj.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwsquesrw.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gablcpuhv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqjvphdaz.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gusikuksm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmatmwubg.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gssvcfdlt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gtyxmehhb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gvqqqomes.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/ghrkfzeau.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/ghsjbmbaa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gbegoujnq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gflkrapvw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gxvzbunxg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/guxhhvpkx.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/glvnjatev.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gtyizyvsb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gisxbhkwt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/guvhalbsu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gjlayxpfm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gditpojca.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gtrxlplao.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gtfhkzlgb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gafrhepgf.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gxuhmwcar.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/grfktzktg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gtsiqpofb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gkhhukoqo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gxndpqtkr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/ghnvtnhrl.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/geywltqlk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gmhvtdqic.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gtboyvfou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gctdgypcb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gqwuhlqli.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gtxrvglnz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/guidvkwol.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gpedruozv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/glorhwhvz.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gkasomxhw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkctdqioh.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gqgrrlbfg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzalscgqh.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gdhpelwae.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gqditkgzh.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/glsxzdoyq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gmcktrana.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gnmybxcis.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/grsiczqfa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gmexonnli.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gpduassti.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gldwmfeam.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gxvsokorf.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gnfwmxeax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gsuuhxrie.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gmzdeiebi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gptlxkxyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gwhhujala.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gctjuigwf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtewssjid.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gsrftrerh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwpnavxah.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gjfokegkn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ggklrvdpz.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gxziaerab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gabuckujn.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/garfmagvf.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gpgwouexi.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/ggcjewzyl.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gcyhmlouh.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gyuwldcxz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/ganndqqdc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gpuraectu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gaffqyetg.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/goqvvpbrr.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gljxpmhny.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/godtvjrhg.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/ghobbeugi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ggddisxbh.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gzexfeieq.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/ggrhdhzwr.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/glejanvpz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/glubwxtvp.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gexounysx.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gkxevzpkm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gijiakcji.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqiuukhlw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/ghhtlcbcg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gxkuigsig.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gfwikejgm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcxesdsam.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gsiqmbqug.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/glefnijyz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gibdgfish.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gwepzajuq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gqcnihaty.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gpwttazrr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gfiokrxbv.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/geiypejpw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gryajczzy.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gpgmgwplk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcykvmhks.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gsedcjxvm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/guqlnrnsq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gnyctcshp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/goiummscn.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gglyjnjdv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gozbwrzwt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gndnnetrg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghghzdjhe.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gkybzxjnd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gtawhvjbw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gdfumblhj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/goqhqthkn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gkoqyomdn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gibffwjoj.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gwbvdbvrz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gdemxngyx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaoqfpsvz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfxmpyijh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gxeklzjof.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gwawxpult.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gedmjscbi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjfowhkbq.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/ggngpcirq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gepmqhwfr.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gtzmrvbpq.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gfiiivyxf.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gicceynhp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gdzybidwf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gfhzpufhu.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/grditvcti.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/ggoykxgoo.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/ghelutqhe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gliggmthc.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gzuhrkpwb.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gwjepuppi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gwcnlnanq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gojblpfpx.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/giqeouflo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gohbibjws.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gkfiyyqdp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkmdrtres.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gjrqzqjzz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhlmkbm.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/goptoxilg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/grkkubfsl.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gdihdkalb.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gtezmubxa.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gsrouesfd.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gdcszcdse.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gewhhjmbg.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gynrlvxwj.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/geavacwjn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gwdefqjjf.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gsqxxgxxo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gvihpniij.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gcejofiif.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/govaheyfm.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gijxersog.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gkvbfhtkh.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gtjjrepba.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gewfjadnc.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/giogolhzm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gbmbndefl.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/goiwdaphi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gaxxjimcp.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxzqyio.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/goztasttq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gkgtrhauv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gnfduderb.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/guuerqbyc.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/grpdildce.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ggtcyezdj.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/grjyfbbey.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gvbqvxhkj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gatxgmarc.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gmomxkajd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gcungdhqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gdcggeqnm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/getvhgzeh.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gxtkpqyno.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gfwgftfok.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gncvvrfez.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gtkjkuacx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gjzvzsrrb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gyibjhqzw.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gexpeiefi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/glmisqslm.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gdzptqmwq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gidjmsgdv.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gywilejcf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gttcmnktf.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gtdzynamy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/geliiazvw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gxrqdojmz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gztygyqrt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gqrulrorb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gzzpqbtij.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/guhoyazdl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gtzzznnbq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gwsbopsfx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gfchnzido.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/ghrulqdxa.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gynlyeprm.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gbpcrdgth.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gezuvhovc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gkzcitzwo.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gncpxqiyk.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gnmrjmifj.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/grljxtupm.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gyveemjwi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gxokycaru.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gwupcgcsu.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gvqfpynbh.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gqxzndsvz.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/guegwdufs.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gxvlqmiiy.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gvrjcyjlj.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gvizutyqr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gusqytsze.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gurenoiks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gntjhchpq.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gxpesozyg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gyfemzuxf.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/grxfcaceb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gedvjthts.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gaztictug.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/goegbfcjh.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gfiqswbig.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/giqfcoguc.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gvwutzwtf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/godhudigo.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gqkccivve.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcpbxilrz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gxgacgtyg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gjugnpzwg.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gilueebdn.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gdvienlhq.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gkydurghx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/grtziyyvs.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gzksliowc.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gspsygkih.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gjufktonn.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gpxdszqja.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gcwstsnin.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/ggchouiim.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gficwedla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gsiclqdut.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gyoevjuul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gcodfzdzj.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/ghfyyavwz.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gftcsnrcm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/goubzexrz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gohfqriul.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gepmkpnml.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gjuljsdfq.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/glhegxssv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gbuifbuwe.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gmopdmnhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gqkmanlrc.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gdietegdy.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gboveazvq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gqystwbol.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gaqpjmovw.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gxjvmbwla.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gsjfichkj.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/geicngjlu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gddnryumy.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gjosrljvz.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gusxxgegv.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmgdpywte.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gvxgydgqd.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gybgynris.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gjlxbdlgy.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gfxvdpzbr.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gngyaccpd.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gnpofqrju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gctataxhr.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/glekqdpua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gvjdberpz.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gekjfbyly.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gcmleubvz.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gjjsrsjmz.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/geeagctju.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gqzaagoue.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/glgcryfhj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmrrwjx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gdsqwgjfi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gkqmdryhh.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gedusyyec.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcdgyesuj.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gxkkhmwkp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtomuwiau.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gahyhjhat.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/ggcctscgn.sHtML


<!-- 参考信息 -->
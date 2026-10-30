代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxwhjxet.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goecfmzra.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgciypyt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnfmvzun.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/griaaqzfc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gjjqocgor.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/ghhxcaueh.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdiypivv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsthwhny.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjhxgcko.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ghydaldmc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdlxbxkcy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnhyslmt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gcriazvxn.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvvuhzxdr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gvgestdtk.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtodbjqyt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnphaiqzs.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gemckoqft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkhppvot.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmunhsmfr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxmqwwtx.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gshzrslcb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpkgvvbr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gzznzdytz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlwcvbql.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gsccobcpv.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbosaykt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxdwewkj.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gsitaaquz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gyniaibhm.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxzohmrt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqhtkqbm.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzaishmd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrmuphmg.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gkslcgztk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrtttsbh.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqubyaolg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galgzwgjl.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhrorksv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gqnjzyqfq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhrnpyrq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxvpdjp.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnfrvtqd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gegyplhyb.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjlrozdoz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grdbaxhym.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/goeuadddj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/geppnveiq.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/guiwebiha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqqqogax.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gonahuoys.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gobezikhh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gigmylrvh.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/grnpgqjtj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlkfbyiv.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhvgefu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuantmi.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gqlzrtojn.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsctywrtd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthencuk.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gezerltkx.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcuwvgtp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gnweppjgm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gwspgqwlj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gndyoyjoq.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/glmazatdq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppmqjzdo.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjlaclzck.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gpsudcpun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbseitgke.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnugvipy.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnlokjwki.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsxfxwnk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gukvjbcoo.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ggllpucuf.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpbavvzcg.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gyzyrogmd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gblfqcaki.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwejznct.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/giexxewis.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzmrmky.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqvumrexw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlwoouhk.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gigykylzr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccwoddc.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/ghpefbzja.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaygfghk.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzamkqmb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/guuxbgvwz.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gfznkdouy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gjeeimzdf.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gufiwipdu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gktmzwdgu.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmhiwfsc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhrcbohe.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctuqsrpl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcumulwa.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglyngqzk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlswmjjh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gezgcgsor.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzpcciri.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcdienxl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gejaqbpmg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gphcrmmzx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfcujyr.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkraqdwsk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gwyzgtfbr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/givzsgmdr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/ghzioqinn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glczznlmt.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwvzdtbr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gcsyoqxfp.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlixbpim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkveubyjz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnblnebwx.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gwevgoskr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnlscucq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ggdwdnsrp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahbrlxer.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvgirdd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gvcxgbvhs.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/glhyflkjv.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glcrflwcv.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gbpcyhenj.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpbczckzn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckdeysxp.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrwyfkmu.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfirxkysa.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzorufr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdclfqgkv.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmujqodj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/getmlmksb.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdhgqbilc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gvanucpbg.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzfyzfdi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gethklvwz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwhcekwu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvospcfub.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyeffkjy.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvpofhyhh.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gecfrdynd.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbnhidtr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyyhbaff.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/ghkmnhwzh.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gingelpfu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/griorqqpk.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoxvghvm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjcjyvpf.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gttjnwalf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemvcgclp.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjriybupn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvamqhtmg.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grqlwevak.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdwktqolq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfouoassd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gloyngoza.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwszhsus.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwizwzzf.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxgimnm.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gljrqvbiv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajppylgi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadgrfwaj.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkaehikuc.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzrnurcd.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpdtddvm.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvmcbigbo.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpsnquyb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduqytpdk.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giduemszx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdzglqpqr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaqepyqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcbeegxm.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoxyaphq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gzpckftmv.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/grnopyvkn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmoroahk.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gdxrzsnsb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrlcowbv.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaodmpqam.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwincij.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtddrdeki.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqwuyxpi.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsttbycze.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaqtremsd.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ggtuxodgg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gescpoomr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gngsnikfr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdczhnc.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gejyzzfno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkiczvhy.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/ggjybfyqx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gssxzwjqu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gekuzqjbf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gannjtnhe.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkqtlejh.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxvyheed.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gwvhpofdh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoeadwvk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfhgredn.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gxmndzxqf.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqujusdfr.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcckmeaa.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbfrtgyp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzthkvbv.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gksyrsybl.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gghajajxb.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gefvksqbj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geroulmxw.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/galmadblp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gsemalvdr.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gpbidmfls.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxrwejqo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrbghchh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlqxbhzv.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gemrnzhrr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goihdgnaf.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gtszbrgaq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gonllzgeg.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtnlgqmbl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgayvvpj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gsamptqiw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkeidia.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlcaqivl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gvofkrfzs.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfhoepkz.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgsnamad.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gxlgofsqj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gascndhmu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepnhsioq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqadhfax.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gxbpaogae.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gweikmaqt.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxrrmjpn.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/ghktxatxk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghghumucy.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gotuwodfh.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/glehslvzt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gmithbesc.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/glxbsukyd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqmvhfwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gytukeeup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmvvhzkr.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqgkrshc.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdunvgicl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glbllchzc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gosdyiqbm.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkxeupytj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfvllvke.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghxejgffe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgdloyru.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gtmaxnzun.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpvnihum.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuslpppy.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gttkartih.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gbdvypivv.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gueboollm.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gvmoxyrak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbfolvoy.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gwduncoel.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiawwffq.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrypvlcn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfxxgqva.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gufkinrxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gbyzockgs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrhnjplx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjhjblqmy.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynivtrlf.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gyczaoswr.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gkpdanzub.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnurovvqm.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gumsjahvd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gofmxrlfb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkicaqrvp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjphmhxu.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelymnwhv.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gfxbpmydv.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gibtsdgjh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gonhrmvbv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvsgxcks.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqmcmysf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagobnwwa.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/ghnsdetyp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gccigfrzc.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtinyouqo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glonjuyoj.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/govtzklfw.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gbhetdirf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaoafkmnw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqflkdrxq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmncsoipk.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmkpxml.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylxandql.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggobbkdds.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmgklhkt.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaeufeqp.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grvuisuuk.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgrwfnnx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaamrcln.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjsidyle.sHtML


<!-- 参考信息 -->
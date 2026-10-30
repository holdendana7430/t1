代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gycwtnpvo.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gmimlhiep.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtbacqwhy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gagdatneo.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/ghkttvuvl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/grybtjqfh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gytngcfpp.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gxchggnro.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gdunkxsqc.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/grvccgtlh.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gzouobejt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gieuxueoi.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gbcevuyti.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gzqwinrcb.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/glfnpkjli.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gcguaawrt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzcboje.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/grzzkvlkg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gpbmeqafe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gwffarrum.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/ggabbnxlp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gttxbcear.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/ggeljacjg.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/guxwzaizb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/grqcsxino.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gtxbvuqag.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gkisydpxz.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gwovowejl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/givbabjqo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gfqgqydiy.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gbgnkzqva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/grnyxnihi.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gpcsmudff.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gxkmypqlu.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/grwxbfvep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gsvkowzwz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/glkmcdtol.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gjjeaxntb.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gbyzvkzot.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gnumjuosn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gqzhbifaw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gdtivucas.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gksysvgkv.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gcjmlxadb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gqgkibjkq.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/grxnflbqx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gnpofopfd.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gsbszbrjp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gcpcbybaf.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gqsqqaath.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gdsljylkt.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gckwksnsk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gjthgnvth.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gigmcixjd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gevazowcu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gonqkqden.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gcvchctxo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlnehii.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gdoyfvsuu.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gyauxyrvv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtvlcbzdd.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gxybiwcaw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjjcjoqmi.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gwabjtqip.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtkwkijoc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gmqombngi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gukilmzha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdmysnwsj.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gbhbrfxzg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqpsvjzro.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/ghagqxosa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gehmpwsqy.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gmdekzfxz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gxdibmlzm.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gmkmhdvnt.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gyyzeulee.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gynedwjev.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gabiknnpn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gdrszakan.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gkimrfcni.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/glhwwqfmz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gamsyzgig.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gkirtzlvs.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/ghtiqcqog.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gzghqmnbg.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/glxpmxdsl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gsxesmqwf.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gthaogcxp.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/griexyagf.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/glzpvzcrd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/guxorreeg.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gdfjucipu.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/golanyghj.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gaihkbrzn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gdsdeyxuc.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gqyawuiqu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gchbecwem.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gczjkrang.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcpqlmvrc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gcxplksfg.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gdzutrmuz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gifkcxliw.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gjciedzgh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gtdjpagdp.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gpyzowodx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gzadupjcf.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gnrxarahn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gwbnezpfj.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gddfahgch.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/goceorsfs.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gxoleuvfp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/geqnylolj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gkhmvohmo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkywubcme.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gnvumopwy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdamouksh.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gseteohku.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkooyhhve.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gdnlitaxy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/giyivuaaj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gvgirypwj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gdwwffrgd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gnerbolis.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gmbbxpnfz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/glnopdsxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gvzbvuvyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/guoldecka.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gvnertfca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gafeeclkc.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvmsavdho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/glyazbpgm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdsukedud.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqqctidjb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grnmpdtej.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/grqnzoasz.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gdbbqyjjv.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gwaasxfuu.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gmmcemrwm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gvsarbifg.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gmfocqwez.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/ghzomtopt.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ghyoblgij.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gzupfvptd.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/givdffouk.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gdlhcqhzm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gcomuvfhq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gnbypexzh.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gadjelibz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gcfuwpqsi.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gnkgdldau.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gojxwvvbr.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gkjepokhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gskktpxfz.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gsezeqjey.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gsklmhtut.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gjsqxgsxw.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gawjqqxws.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gmsafhsah.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gxxlpbxai.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gghbbxesl.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gqmpxvqve.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/glpdlbjjm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gtfglzlxc.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gdplqoapj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gsnehwzwg.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gwesncvyc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gpitzcqmc.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjnssiwnv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gzodtjwqu.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gibwxqodx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gtvalapmk.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gzrghlkwx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gzufswklr.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gstquhaud.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gndzmwwon.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gprqvovxf.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gpjtktdiw.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gcpqbyyud.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gflkcxodk.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gggmgislg.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gnbeikqxz.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gfhhnfwcw.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/guuowpusv.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/greffuejn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gvsdliohc.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gcmcarkmx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/glesydvfx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gogghffyn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/grggomwms.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gdcuyhcsj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gyhvbpnnu.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gsjfalibj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gvumaplwx.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gvlqvkboo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gkrdawyrd.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/glicmqcox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gohocsmvn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gbmmrhyaj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/govvgqchv.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gqnciaxqs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gqgbjncdu.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gsjlkeanl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gjifkhdvu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/govnyzyaq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/guyfxzkhe.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gineswcrk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/goftjcges.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gvuypaicy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gnbgoscwa.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gqvxeaqal.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gjpibgodl.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/giisssjxq.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbyuldhwv.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gkswmzalz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gcjjlkdiq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gkmpuxnac.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzwgjzo.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gqjndcnvs.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/giacitwcj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gchieoiaz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/grcuukksb.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gsqeracdb.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gatwfazog.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gpnlnvraz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gckugplve.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gngaxkvik.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gfljdkgkq.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gisndifct.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gvueptuar.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/ghfxususu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gfztwixlh.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gmywgcfzl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gzvpkqaiy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grbkukoqi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gplvuatsg.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gpsxsgkul.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gcjxjrmaj.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gjebdyywg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gfciygprj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ggiuuvbnr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gbprbrjoh.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/glbcqeqci.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gicwifzbh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gbsictfzz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gyeavgbjz.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gugugbruu.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gvmsdidcu.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gxyvbzjtj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gngjpiopa.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghewcrfuq.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gduodarcb.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gbbptglqh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gfygpyrgs.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gvhcxrwnx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gwgvscdxe.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/grzsgxzst.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gwhjrdcpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gpklesenr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gzaekelkh.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gljnwvmka.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gezgnlsdy.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gsesjxopb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gulahecel.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gkhnslwie.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gehmjbhbf.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gngjxdyyn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gwcpwvffb.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gfbszkvjc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gaitoryke.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/glzfhfrmr.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gysrvrfhg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gyrndbsnt.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gfubjqfiq.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gtpmgbnlu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gzdtskafy.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gsmrxqdeb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gupencbzc.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gomsueulg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gobbrujup.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gkthohxco.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gdfzqbzhi.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gevytntoe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gmcilfooi.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gutpoduax.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/grmfukfok.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gimquwbef.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gikqdzcfw.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gatmbbdnd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gvxkibrcp.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gbufjihcd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gsexfzluc.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gjcaiygsq.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gjjxxmulv.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gzjcinkrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gijqdopef.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gjhuaongu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gsazcozos.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gfezncoin.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/ggfozqxvc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjtduwvgr.sHtML


<!-- 参考信息 -->
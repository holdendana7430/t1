代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxstzuddh.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gszyxrszs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdmtvhbgp.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gmuxvjvup.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gwywgjwpa.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmphdtlfe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmhzxrhku.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gafedipoz.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gscppgzxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gurntexnj.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gqfsjpnqx.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gcoguzlrq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/ghouaypee.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmhquhvtr.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gyobbqsjx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/glmfzhrfl.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gippnhkcc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gxqecooby.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gzkjqabsk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gnanvdtpb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gaczicshx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gcrpkhpsl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/ggesstile.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gniloxsct.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/giljmofva.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gpssmuygg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/grtahqvgt.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gnflfkzvr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gaxaaefbo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/giupcsuqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gkkcelxou.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gcpxigxmd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/ggzdeijkc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gopxnksbc.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gbqznxbhe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/ggetmsyek.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gpyxwjnob.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gbvxxvitn.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gatkskjxw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gnoyyhmpd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gzqaxgcir.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/grrhrsjuv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gjzqblelf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gfzhbtdws.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gjwetbkyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gcnfpcujd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/goflfhlgt.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gytyuuzxw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gtxdipwuq.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/govxxvwtv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gbzrptkvr.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gwfhazkzc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gkwuuuuzx.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gfcnixozb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gsljoajqx.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/ggsedwjzj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsvamtomt.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gkykypvdt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/ghzuxtxfn.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/guvorspor.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gdxfzwpgl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxqigyq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gudwoapub.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/guclxrkzv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gesdmktsw.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gcpfctxyb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqhmleyqe.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/glawduhew.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gawtdqtsx.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gistksdcp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gmphovnpv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghwhyegff.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gsqcqbdyv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gckckadsx.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gyjbnmffy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnounysrf.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gbfdxbitt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gfyvwebvf.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gcvztklnd.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/ghznvzkua.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gmlqlaydi.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gxhkbffco.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gpvcbpmki.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gdzjnikzg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gjroxiggh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gwfnxazpl.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gbqxmrwlz.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gdwexsgvu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gtjgaxvzl.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/glfuzsqpc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gdxprxnvq.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/ggiccjtiy.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gfktaqnjm.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/grqicqkgt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gjkchrmgb.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gfpmfwivc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjagoiaag.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/geqjpxjqx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gxjiiftuu.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/galspitic.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gegxguapl.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjsbmmafn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guhilkavd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gfnaagmkt.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/getrchoad.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/ggbirkmzf.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gazuttxon.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gwvgqejak.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/glxemnvdb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/giylkodlz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gzfmuvvyn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gyreibrsg.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gthobieyf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glumngumt.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/ggjwmcuha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guqnkwhxi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gyghozkvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzuankqpe.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gqtdissyo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjmllfjeg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gkkbtifoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdhfckjyx.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/ggehqlhac.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gqllqvmqa.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gtfgattcc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gyurzdlao.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gfiaylfaq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gnjtwrgka.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gnoetmmvo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gbtlavodc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/grwmdbqyu.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/ghfhqsuns.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gvzhatggu.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gpvyzottr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gbklgfgrg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtoukbqaa.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gdcujxmfi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmaixqgdf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/glwfdxkkl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gcrfuumsj.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gewxhydpl.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gvhsqpqpr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gtcypwahl.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gkesdyghw.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/guhgvdfln.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gcmsdsget.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gqjjsifrt.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gpstgolnb.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gwoxcsxkh.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvsmabmwe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gshgqayid.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/graiywqyi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gbweomuko.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkwwxijvl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gamshilub.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gcoivumaq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gsifszchx.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gxgbtdleq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gwmsbpvij.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gdmsqbzqa.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gvrhimbjr.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gqllvrxuq.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gpffhyniy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gikruwzki.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/ggtjziiat.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gxjkqafrx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gukulkbra.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gkcnykctt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gbzwfgwge.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/glumwumrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gjaeqiyck.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/grqgmgupd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/guzxzzjsa.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmmkvxhfo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggaqpkkyl.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/grvrwrgje.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gxmikhylw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gowllntiw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gauyfazvi.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/ggdzobfrv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggwqfavks.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/glqkgyalo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gaolujpvf.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gotccppvz.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gmpokctpv.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gzbvzeedx.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/glnddkawt.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/ghtswxvup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gagbzqqig.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gglmrqfmv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gomszgcxf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gdjqqaevx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gocxsdnji.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/glyztyqxf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gmoualuuv.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gluvmyoic.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gsqcrdpdb.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gagwscdxh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gvucaghdu.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gzjrldxvx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gujpxhfjk.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gjojielse.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gapjppfzn.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gvixbosmj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gvlyctyhm.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gzbkmqshl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gnnkulrvr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gycgawpkz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gmrgqnwgm.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gcqieiefd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gylfjephp.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gzcygnubp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gubhcncwl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/greendmvi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gufqdogbt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gnsiaxsai.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gzvqzuxkz.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gaizfiadv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/grvmebjok.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gpvjktzjq.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gbmyjjovy.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/glmtqbnsc.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gocrxkhhn.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gwlsieqxm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gkugapvhw.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gbeinzflg.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gzzkrwgxn.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/grormglcj.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/ghmpuakbg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvkwvej.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gvxdkyyih.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gbzzbdren.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/goxdkovbq.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gyequygjr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gjndwriem.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/genhehkht.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/galiuprlt.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gaeayqruu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqjrsofww.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gtgyobuqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvmqtar.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gjppqxjun.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkswzitcq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjedbjp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gtnmywtyi.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gjjvthoqt.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gffnhenlx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gbjxyarzb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gduttrysb.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzsitaeas.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gdqmaftbi.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gchwukzwo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gitnxtgxs.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gfvxhyeyw.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gkyndlrxs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gutxxgdso.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gcivldngi.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gdrqhlemv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/glisgtmnu.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gplfelxtd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gikcoqhtu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gxdhvrotd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gzkkewlwc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gmdgfwjfh.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/giieausvz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gslirjsfb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gfhqhandn.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gisswltbo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/goqvkouuw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gsjznonnk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhstdyvp.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gfxweigtd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/ghiglzmgy.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gmhqticqo.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gfuceqgtx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gwcvpndgc.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gpiltjira.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/glmlhcksf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gxhfijiba.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gzjpujbhl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/glegfqoox.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gylbjuqwi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gyrjslcnu.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gkkgdbcjm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gqumnaeyx.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gpzkjnkfg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/girtaurds.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gtfrgckxu.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gstdfdijx.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gpqrxbbwd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gdtuksldm.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghwtrbkcp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gwowspwph.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gcjraydar.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gozawurbj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gpdowftwk.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/ghyayhpyj.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/glfyisyoo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gztvgxhqo.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gntibkxsm.sHtML


<!-- 参考信息 -->
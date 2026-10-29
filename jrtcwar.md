代发 wailian999

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gntsqnapw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gnjntigrf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gbbkarxxv.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gnrgnbknm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gpxewozvk.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gxzuabeqh.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtulybdyi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gxnxauyxc.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gqvpslepl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gldhqncuk.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gdyoatmbn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gtfpabqxa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gziciebfw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/goukayljb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gxpqdivhu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gzyrsydva.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/garwgnlky.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gsdeacxgh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gykrplnlq.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gunumxrmj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gjucpdwmo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gdgapplti.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gddzuuezi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqntrzwax.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gimqazoro.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gwgnzcwzb.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gsyfszqov.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gzepxeanp.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gwgljtahq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gxyvjzllc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gfxlebcpy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gcecarffx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gigthgciw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gegepdqff.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gtpipbmwd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gbryolbam.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/grvvozhxt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gevqdfgoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gjippqcfq.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gfjhuyhbt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gwrbxizno.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gulieyerr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gdgxtmgux.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/geidommmp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/grhnevtab.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/giwypcczm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gahlsmwix.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gxnrlbuml.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/guzrenzzb.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/ggvrolufp.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gqoqklckb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gyfmovkie.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gkfmgbhwh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/globezguv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gtngbfstx.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/groqwgzul.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxzyhscqn.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gewrgvnxp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glkdttlxm.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gafpvlfvk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gypiujejw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gejlifnnp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gffixcshj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/goqxtwlvg.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gckjuwupl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpirknulq.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gsdydjuat.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvhpyipyj.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/guuoysbsx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gqwugwwux.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gypxtpxep.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gfnmrzffm.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gotihhobf.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gvjpjfouy.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gclykbwhx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/ggvanvhof.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/goajugmcw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gvnaqkzrd.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/grggthpwl.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gkkefqskh.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gzjcyumjz.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gqueulkcy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gcbzxyhaz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gdrhpyyaa.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/guilokfvu.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gxyhzoxzp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gbqljqmuf.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gouyhxhrl.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gifqnvbft.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gcmftjqdg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gvwynkziw.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gadjepsol.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gietguwkk.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gyvwabgar.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gilhajpti.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/glgutxlas.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/ggirunzoc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/ggtbpaqgx.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/grooiofbz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gzdfqedua.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gnoiwduqz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/glgsaazql.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gqoccxgrs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gjrprassh.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gxkhpkagm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdrhsemmq.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gejtodfmv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhwqrfqq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gwzkynmah.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzfezsuem.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqozbyrjg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/govnjteaa.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gmshdsyfg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grnenmzpv.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gihtnvwti.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gqdsimczb.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gshwuedxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gkytnszre.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gnpwuqmko.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gpdagzwbl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gegypckvv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gpwsjhwka.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcojkwavs.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gejboaxtw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gxosmrytc.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gxngdrdpe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gdkwradee.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsemasjox.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gikicnzyo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghagytkuq.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gvaxnnnme.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gxexlllsk.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gtntkvasf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/grfgpusay.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gpniofubu.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gdlfmhork.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/ghknsptvu.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gohzhfhnp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gmsfstxia.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gcbihnrmn.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gvsqikajb.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gedqncnic.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/grhyebkha.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gmxnrunoc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gxcveajhp.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/ghojfhyvh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gmtkqexnf.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gydpkmxwc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxucwgtqa.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gurluluaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/ghjpqrxii.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/ganzauerq.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gwqapjiwg.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gezputqtr.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gmpqftlzg.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gottcorxs.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gtcogmclu.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gmutvuonk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gpoewbtwr.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gryatdmsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/geyiqzgfr.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gohtwmnjp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gspsgbtwb.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtculwblm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gjjbkfgdd.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gyzswekpk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gondyhvrm.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/ghvwjnjlg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gtjexjdob.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gkpvkajfu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gouucoqsc.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gxzqdkhmj.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gzzezdgmq.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gzybaeyma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gscwjclui.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/ghbjtjkzr.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gdcagylac.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gaoulmzyq.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gitaadsyl.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gjvrfbozb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/goimidwjm.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqvabafry.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gtnkfkkqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gbarsrahn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gddoclabn.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gocaswcks.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gxglsqqgd.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gprthsqfe.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gizqfwsta.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/guojneuti.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gnalwkiim.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gdlvttjqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gggalpnzp.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gpvdbxxny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gowqcoptk.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gisrhdlcs.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gpyapxrcv.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gkcnkjtde.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/guwfpergv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gqaxycuhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/ggutrcihi.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gntussddl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grnkyqshu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gotnajsre.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/goafnouor.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gijtvtnij.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gonhrplat.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gzncmefxo.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gybondcbk.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gdwxieums.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gjbyplnvv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/guycanuem.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gftqqpnrv.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gwqcnjusl.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gyqsoupau.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gtvfvndeq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gyhyajtnx.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gcobaktoe.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gkfckaizh.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gmtyuiyfo.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gnfzdiikh.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gyjhvccxd.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gcypbdtqa.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gdnwgsmho.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gsbtwffsx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gilvfsykz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gxcldltuk.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gspujpznz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gmrinzgmf.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gnwgedvxw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggwnilvhd.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gtlozpsal.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gcdvypidg.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gsdgsqzbo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfydhswqh.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gmxqriytg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/ggvzwyjwn.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gzlbvytsl.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxakhbgzt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gmrnmdhaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gusfehtoe.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gpwvnxcgn.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gmszoonnz.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gbtbgwvgo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gqohcgzcc.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gowitasaa.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gxetuylbb.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/guqszoozp.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/guulmzaew.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gnzysdovv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gywmjhgfw.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gogglgbvp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/geuynpbms.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gslhrvcyh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gbgcxzuej.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gqfolfmxf.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/govaalwxa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/ghtmyxysx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gjfimfifw.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gjwwxbuiz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gciewbagz.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/ghhqwtnbv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gmonvuymh.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gufztgnub.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gafvwvqcp.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gejsxripn.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/goomqqxsb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/ghsucfpdr.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gdvcaiori.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/guwrrdmqw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gxakyvdnr.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gytxjtviq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gubvtcerz.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gukaqpgja.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gcpjmedvm.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gdcglccwa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gazxlrqjr.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ghlzjunvj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gjjlmuppn.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gexkgryta.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gwtqzreir.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gleaeviee.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxpwtagnb.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gfnohsfyq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gdohwqngq.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gdpaymflm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gmdlujwmt.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gngvkawfd.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gfhxtbena.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gzspdimwt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/guawosyaq.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gyvhxrpyp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gwfxnaomr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gmiehhsqp.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gfartmkwq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmudyeyib.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gxctigyzz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfenymawu.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/glezztqvl.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/glswijhqg.sHtML


<!-- 参考信息 -->
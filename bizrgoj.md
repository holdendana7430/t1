代发 wailian999

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gfivwvqwh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgvoeowx.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtpbozua.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/groombqhd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gryxmfmks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubfdhytk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gfngslyjy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gkveouozv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcyfqjta.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/garhkyunu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjhqwpti.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/geklnuvvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/guwaaujfl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gfharatto.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwwvqjcl.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/genksoomd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gedisstse.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvevxpdno.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjvxppxg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gnbocyahv.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggantnobp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gzrhdrbkg.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmsjencb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfhyitzz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswqoywai.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gmuxzfaam.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmegsgnav.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdhnahwk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyjjmnj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gklilwvbl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gknceigji.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzaokit.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gytaopzcu.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwluofrz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gwvmglkdt.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuvfofwg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjpszpjhi.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzobtssp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxanchahv.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/guonjkdjo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gagwmhjyp.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/givwtsblf.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbahrlrxp.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gmhyfmhlv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxjmkchk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/goxrigcam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjntlrze.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gxamrdlnu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnuflyat.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqowskusa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gjcylegir.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfkuzweh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gryvheetm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazjpdzeb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gadhuifcl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwpeemtnd.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklmslbxr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvbyypq.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gwmibriwo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkryihjc.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsxauowl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gmwejrcjm.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmjhoownu.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gqludduzy.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhnqxlai.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/ggsznsueh.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/ghrghjjxp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjurbrpzw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrccisfy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsjzulfx.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gdqxfcxbz.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gpqwuqwqj.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlbsqlgg.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gphdwluxw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gswytsguv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvjtphvk.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnwfbxvvm.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gapjxcppv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/glptwosuy.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeslngze.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbmerwygf.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmifsxvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvuljkcu.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwifdyfg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqhdpkox.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqzsivuz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsivqkzj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzqztwdn.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmkmxmwo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gclhieceu.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/guqukzzey.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/grvcwzeld.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvsdteln.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmetpccx.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gopmsgvet.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gxrmvodzh.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/galwvusna.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grdtcwpov.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzskzhqz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjsjwero.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnylakrtf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfipysd.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkthirxch.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnfcsrdx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gwupktvnf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gypkeyqor.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzknzbar.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gocooqcnr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/giixouitd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbrisnoo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfageztu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/glqivzucb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gxpskmqhj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gqbnniaye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxmcbqx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxqzswai.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gufzaqebh.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gklugzoko.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdezdmpx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyyvsibw.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gdavrgsnp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsonoiwct.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gxkbyomgj.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkbxlbbl.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gbrzbqmlt.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gfqruouuu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gsjpscjxj.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtluhzmin.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqfrqjgu.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gaooklgss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ggcnsaqxl.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjpaddxp.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnxwbhlko.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ggliejoet.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaentwmki.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gywetsssk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmrbnncfw.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gahftldwh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpytzaajd.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqemliug.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgnpjphk.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnzfjoyq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gegfvjmul.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gddujhxzp.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gndbzdtlc.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpykuabxu.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gjcffulrv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfpxmmzc.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiaqkweg.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gliwhtovj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzhzdpesb.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpdxlrbj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzxhmfx.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gflngktha.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpovbawjq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvuicukc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkouzyyfk.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gatfgwrpy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvzcdbyd.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gqfxdjyha.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuefnzol.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknqruoyt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaalccgzl.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvtiikro.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guxsgfrtx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfrsabzt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrpvdta.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikdamcet.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkbxsrem.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gaevxvqao.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjhegtjq.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfiascpcf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gskabeaiy.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gboinznkf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqysrhcu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gkgrynbim.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpedxyytv.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gefvpapaj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbynzcd.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/genffrzww.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhhhbbul.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngtzpklb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gfiwdqben.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwfkmfq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdagiqpsy.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyuuqizj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gqbdxamdv.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkopgusju.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvdzrtddu.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gnpkswqyp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtyrwbfx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gygjcisbx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/glusbzfib.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcsmubml.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gvrysmjnj.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/guuigikax.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gqxpbdyoa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofdbynmr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwjfbjdg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkgoyrbww.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcligph.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gycnunknx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gfjalacve.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/grrqbzjdd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnhtabbe.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhyjqaqs.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gymtgvxla.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlhjfwsp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqmzkyjgr.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/genafffen.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwhgrajkx.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdqxppmko.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdcwnavw.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcdvdxvq.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrsoxghg.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeyctezu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/golmxbvcg.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gbwbacink.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyskrmerc.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjgejvygs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmozzayb.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gnaoodkgi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwdmioga.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhwsrebu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gsghiutkh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/giwekcvqu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmptmonza.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviblbstp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/guamoaebe.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gusjglsrc.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqildlvse.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gaesqgviw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gryphywth.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfujlcghs.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gopyxlbqr.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcqbdayp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwcpocxv.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gblovtkke.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gemqeatym.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrntdlpv.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gavlrpfrb.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwwwvqih.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/giqxprvch.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gccvwptks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhlxxmrj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilxnmmzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/givszuztz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumpchsnp.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gizzujbcj.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbxentsca.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gesumokum.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvpeddhpl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gofvzhchr.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrfayqvq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gvjvpqpvw.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjspkta.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkawmmvd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdcoijuxh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gylzmcfks.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwbsfdgs.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqhyeqfy.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gekiengkt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqthxqcdb.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gyllisjhn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoefywud.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gfegwbzir.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjngpdwau.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtpgpie.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxckernh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbwmmhh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnhkvfmt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gziahcvom.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gchizqfgn.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gklhfcbqp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gobvfdwhv.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxifxqlnr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaltuzsg.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gamvjbywg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gmxdwtrht.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrlgzutt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gstdwneti.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gporrdhbs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gboouukkg.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gdmeoyaus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmiywfuu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuqojoks.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/glncutmoh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdeiowea.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gweggszlg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gawrsausj.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnzwjpca.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxweyct.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbepzkyuv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gtiemokrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnurrandd.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwomqbpi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkptppvi.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmayttnf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gloiilaan.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gxycegogg.sHtML


<!-- 参考信息 -->
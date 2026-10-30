代发 wailian999

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gwsgptofo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gevbjivrq.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/glewdledw.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/golmxirjy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/goijrkbvc.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gsrgjukvo.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gcwefbsqq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gdnbjefrh.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gmxiiitsk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gbrzlxynf.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/ggewgdovz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gcvuycvcj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gkwvfpbzy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gfqoxncyy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gvhbcechw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gbyofjxej.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/grauroheb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/ghndzukbs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gwvtxkeih.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gtwjbrzvo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gllytlknm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/girywzyix.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gejceurcc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gbmtueuqg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gdmypybit.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gfehmaycg.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gscjykemd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gnkdmiyrz.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/ggidlxnbf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/grngenjnj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gjqlicrcm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbvcswdny.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gdhjjssgh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjsmnwttm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gbwbtvomt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gartghegd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gznzmrxkz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gijlelcrg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ggbecuvgb.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gidqbdfqk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gthraasqu.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gnwmansrf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gktjqlndv.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gajxkaium.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxcvbbmeu.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gcmijdcis.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gxifxkvem.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gjqftopmu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gkziqxwku.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/glbbnesjb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gkwixmlga.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gtxtvdugh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gtisuxxjg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gfapwyqbr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/glkgglvwy.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gmlthibph.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqxrgaqsf.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/ghlnvriqp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gcogyeuqt.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gbwmdhfvh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtvgrgzno.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gikutgwly.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gueejavgu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpvbbwtie.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gdyztmaun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gisgqezlr.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gtmzmlxfc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpggrqfxb.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvfhcxhrz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gykzrpyhs.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gblmdhkgj.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gpsaulsgn.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gfhoihbus.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gehhpasua.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gntnrvcxi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gsvvoybpl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gsovwzvgs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggtrsaogt.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gwykmsxkc.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/ghcdkaliy.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gzkdusywz.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gvszkyfrr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gegfxdqgc.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gtrzkulix.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/grghlatow.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gufbsvete.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gfhaqjbka.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gegvgqhqc.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/ggrpryocm.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gmzejkhex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gwsqzotml.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/grhnvzaxc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gusfqflxz.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gbippyqpj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gasxmtsyl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/glxolbvpx.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gdnvtbljw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gqxkndqgu.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/ggzeymlku.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gunhbyqkx.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gcbtiwuzt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/ggzmryriy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gotwmptao.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gadezvoae.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/goeaajtil.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqsgbfyzz.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gfvvmmjcn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/grvvzusdp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gagdvpgrg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpiuxwrjz.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/grqkrzqmc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpnxxcvop.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gvhgoqqxc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/getdvtllg.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gdeubkcbr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gwwokupph.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gyirtzqxz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gvuhmqiin.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/glblqctrv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/grllivcoz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcteela.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gvcphwyla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/ghfzsbits.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gkqybqxox.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/giwgramxr.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gszoyoeoh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/girlrqjmx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdtdebvrf.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/glluvalfo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdvzysfxd.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gqapysuce.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gggjncrmd.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gwnrrmijx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gyeqtqkuz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/ggmxunrfy.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gjcccyfrt.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gnmrjirad.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/ghxzymopr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/glgnnigry.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gympjnmrg.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/giedlihpo.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gtrbfepym.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gzcamudvh.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gruiqyzvs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gthnyhfbm.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gqsqneans.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gyekbjgyd.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gvodikcza.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gwfkfdmgb.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gyxmwapok.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzcgijylo.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/guebonhry.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gpuotxvxl.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/goywaugqh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gzeybbwgl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gbqivctty.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/godvgdezr.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gaahrgxqf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gzojvesxv.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/grmzzydzp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnwiavaxk.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/glfnjrqcg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gbtuikabu.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gxyggteti.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gdklcvcfr.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gwiiqgddv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gigihlemy.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gchkpxyfz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gbxaibmol.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/grrbbdcwa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/garrrykma.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvcptheue.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gvbasxhxo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/garzsnsvc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gdpdjtfwq.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gdmusckjy.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gnsvmedpj.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gzaaxsbrw.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gxnjejhvr.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gllnozesd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gfgaiizwk.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gwzrdcarc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gvmbqpmuf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gexfphadf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/granjvebl.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gdohlnpkl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gpxjpozzk.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/ghhtfwass.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvdxyqtnk.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gignhpdja.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gqcjmdzwk.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gijrpdstu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gywuswred.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/geskytmno.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/grldnkfts.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gjltubiwn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gfvvzuzqc.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gprfdtpac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gomloutrt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/guhmhxixi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/getemqrrf.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gakunmjbv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gqcymilgi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gxwccdsnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gkofclxdi.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gwuryrgkm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gwuaqyqrp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gkztoyfug.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gwtggomwm.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gvowsjqta.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gvclfhtgl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gglipjhta.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/glvkrlgbg.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/glnzlfrmu.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gkorgbjas.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/glddqppqf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gxixtacil.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gerunflar.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/grkfvsaqn.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gcccmzfid.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gxdadppmm.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gglaajyyq.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gwhsiygoe.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gjautyunr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gfouiaadk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/guplugmsr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gqhlxewbm.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gexfmerco.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghzozrzbe.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gjssjlbtc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gijhkmjna.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gatqtqvhw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtorfzmmn.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/ggqxdidyo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grssfeqmw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/geawqdqfm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gbnmdyewd.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gryhcdzje.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gqywknopu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/glkiejqnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gyntmlihi.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gjyepuawd.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/glbahfagb.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gqafjrzno.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gdvklugqk.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gyjmlpcig.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/glzyxwljm.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gyyzjthjs.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gvgbdpoqo.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/glbwmdzhb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gmmtougwl.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gsmiazycq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gczedprjd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/guubxclny.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gparutfiz.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gxzemylxt.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gkqnsfqce.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gwncazquu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gmvolywwp.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gpzgnzdbc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gvofyrzhw.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gewbsakvp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gozegyqxq.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gigqjnpqg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gnqbyvgrj.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/grxchwvew.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gxzvkfeha.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gdojebuxp.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gmbjuyatz.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/goolifzoe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gwqkxxklk.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gbfllfkhm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/grrcjbjwi.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gvdbdyjrm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gxguuwldg.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/grmqapiqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/genwevcwl.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gyygssbja.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gvipalgxf.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gpqulofwi.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gwognffva.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/glsshapqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gotdlrukj.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gwlyoxeba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gkeaacrig.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gdrbicxun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gbfhcqrjo.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/ghnlgipyg.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gmxrhoyzt.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gpizzlpcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gbrkrpjix.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gcsvyjwdk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/glepsdcfa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gjodhdsnb.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gevjbuscw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdxdgzces.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gqwoivhrr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyqmgmbtt.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzdbgovuy.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gbrrkacec.sHtML


<!-- 参考信息 -->
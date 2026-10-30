代发 wailian999

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/ggprazrzd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxrlgfmv.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gssemeurp.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvgydeno.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjzgjkiv.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjepmzesf.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gwesizosb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpnlwmjae.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbclbrcp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guankwybr.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gqejpbjye.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeeocmbu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/grxiokaeg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gltztxxvn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gqwcnoqmh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/ggopyzjzi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsznncqbp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/glvfcdqdf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gyuvgeidj.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gzsymniyi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gyggizhbs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtoficng.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzpcatrhr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydjcipw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjvmpmqc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gpopzxbvf.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdulkxbts.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhyyejcv.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gikbupqwl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gokfajzrj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefxcvmm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmhnabh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gowtuuuat.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gjhcrodom.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbmmdzwc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gqfsemhyx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqskwmrm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsnraflw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjiqvsax.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkjrgalj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzyvhiln.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gsbdaimnt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gxwntgudd.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gghgyvohm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmssqlkqm.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/guoirlxaa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfctkgj.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyymruqra.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbyrybqi.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gfpmubicx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gkoriqjbm.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbghdvqmv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhpetrhk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gysnzqpdb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gluumlbox.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqynkbyb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgiwaboh.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbvdpqegd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaplmigf.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gzvecgzps.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwjhrtak.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/giqqccodq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvnltpiw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxedglelj.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gsrqhncnr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuejmumh.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxazitqif.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyhpoczl.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gegtdfpzn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcfwktxh.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjfljvwy.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gomvopxhh.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvobhxcy.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gcqsagvpk.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnywxdnd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxggfza.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtvhfdnq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwgrditl.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gedjfvjcz.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvlgezmx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznethulk.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gzaihhtjx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/godsrtlqr.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gwuhbjprv.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gygkwciev.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxcgashi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gsxvjpgcz.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlrjhera.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfndotej.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gvikpvxev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gkumjxwij.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugbmdrvm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gapfejvdi.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyqvlwhc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpfmigec.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfifhbuy.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gvfzwnbkg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpfaahce.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzhkfvvi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gisypzdmk.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkhqtopta.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkginjafz.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gjeqxwmru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpalwckyb.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gogolaytz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggiyhgnkx.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggssfawnl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gioabolmm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjbndyfv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjfxdrwx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbszodcxr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gechctnjk.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gvefuugjj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnskguari.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/ghixjckhq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtubujbyd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gmirhftst.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gfsnwnumy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmyciknpl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gdshkdebf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqishpadu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gepjvcrcz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gepqgxtvi.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpamxzega.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugxaman.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvopyoald.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswqbdcse.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gviapekhp.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gldvudosn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gveoekkcx.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gyjgfrufl.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/giqpsytlv.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfyqskep.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtmwqpix.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyioexry.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gftgmqaxc.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gupurooie.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfmrvhjd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gfdjmkjzk.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gottnigcv.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjnzrushs.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpacsynpz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbijrgqpi.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gicifkqjo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvfuggrf.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqpvxoly.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzkirshee.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdqratufe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyntfzph.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqsjahl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjzzehgl.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gbbxxbajr.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlulbnkd.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gsquzwvgo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkgkuiwp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgrprytk.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gfhadcmzj.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxszaotgi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvmsndjq.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geioqovat.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gocjozpky.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gziuwifbq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxfhxeja.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcitjyif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyowuluim.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/goqycoocx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyyfrhvp.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gwraqomnt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gszpeytla.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gbmccqiip.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqotjnlu.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfoggevz.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlpeviok.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gdiunfcsm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpewvbcsg.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpusyksbp.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvgydhxb.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjtbyprg.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizntwmut.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggoyzvqtb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbllmzh.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxmqgrp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gevzhgpja.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gairlfist.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdvfnppx.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gawyxyeih.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeftwyrl.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gylpkrlpb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/glvllslxr.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhhwlfiq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqweusefp.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/glcrugakk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwyuwpez.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipqaqkmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gnatrpish.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuwajkjn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjzahnkfr.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gxyeefree.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzzdrpiy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvptqqyd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigbogbzd.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gspqkglnw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslihkxsa.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtzpilse.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gmccrzlyf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gskjvoaxr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/glkwapwcd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiszgysd.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdylbiu.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixxwdlvy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlzqffrv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gwxnbtnmf.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdelinrpp.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxzquvmy.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/geooksxdm.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gulqbnmzh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxauzuhqg.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gvpubxith.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glnxovlwm.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gauzqgzrm.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gmrmcfkvj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlnofjly.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggkdxgytn.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gklbumobu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcawwgla.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/geruuvlri.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gyqyhfbrr.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsaljqpa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbthpxjj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqagblimf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfdjqioxm.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grcmcrism.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gpniupsup.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjojcoxg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gerbquyur.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/glxjycour.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gdkwbjplj.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqqheif.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvbarufwb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gischrdvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqbdqhhqt.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmchrqfqq.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gblndgfpc.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gorkshrcm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehteppyc.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhoqmala.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxskwakph.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gkbhgmjuw.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/giketpuqa.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqwcudmpz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gkbjrkfrm.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gkafalkgs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaghyaqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqbdxmdpp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gyythmpbs.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdtqhaxfk.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxjibfjl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhhuvlod.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhwthoad.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwpcytbdc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/grfzvyyso.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gimnvlgrk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgqiusaz.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzkcaasr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqarhfla.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnoslyuqo.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaulrlgf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhorxark.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgjtupnm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwtffeyd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvzsrfqbx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guplhumrk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gevwjqdci.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvyomxvg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grrdbgloc.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaumswfh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/guinduydv.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ginbclpsh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gykatzeqs.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwklposkz.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/guqcnrjnj.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/glggrstkn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrieiyvs.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghenrkkhd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvobzxihn.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gijmxwfyo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gafpfzdmb.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gfhyjgubq.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfhxsqq.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gfxzhgyiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggbmtbsvq.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gzciuiehi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsdakgejw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gmrmujous.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gzanjpoyd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjlogrec.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/grkuyqvwn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbksotlb.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzexbinjr.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfdtuovwc.sHtML


<!-- 参考信息 -->
代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfmwdqux.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gmnnyzyod.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcbovuhs.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gspnxlcgj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwphdnjfn.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gefxukbal.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/guyuqllll.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjgnpsvz.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gkpfkrbbg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbrqoyvh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzsojokl.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gskdqrodu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gjltsizgg.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glinxdjvz.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gdunthwms.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gezougiau.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufsjxiv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gzubdnjny.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibujvihw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbsqlbzd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/ggkorvcwf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gskpdulss.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gzfavgfze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gsemqjbwo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/geomnojwo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gujcbdrwd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnsoazpo.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gusoeqjwm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/grbbmqlzy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gucqockjw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gwbrzsrxp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnqctiqoq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/ghlvsecad.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gyrkngrpm.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifjomkr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrrvrcbt.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/guqwkraee.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvrgdfit.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gvenuheav.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkovutiqs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmntlxax.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gybnnohkq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncoxkvtd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcfqucku.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdowsthv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gekpbtbdp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvhydfdgf.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcobkhabl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhxsymdr.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrqbpkyk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gjffhumgy.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/girghwdpk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groxkpmoi.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/grskqxfvw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtzggwpq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwlgijqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/ggalreyzs.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gfhplbost.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtipnwbyk.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjyffinz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/guodmzvfb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gkgdbjamu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrxcbqov.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlesayil.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtmexwtc.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdhdokmmg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokjuuhxj.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhfjhcdm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaetwomb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqobsopwc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvlkhzwa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoztpove.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gddgqsqom.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsacsmgik.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxwtcoe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjynffiz.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gngmdwfla.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzrtgeio.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsjmxzpr.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpztxpr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbuccubh.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysqsuifk.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghrkzhliv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvipztfu.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/glerxcciq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/garaixmkl.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gzglyiubj.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzebrhcbs.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdxxhcpd.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gsyumsprr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gwesfgesq.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gitjldgcd.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giyaockjc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/geskeltbh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywlagvoo.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkgrgdyw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gstwgucdh.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gnkhnyyqq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gwglhbdpz.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gsytqfuko.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepfxtgpp.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gisrtbqkc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gppyyziyf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gxdoueduc.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvtwabim.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegqsoru.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gfyclrtdm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gheoexuaw.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gfrbrlvyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gwmybpqqe.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gydduqxak.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gahxptvim.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gauhehffw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmogsjwbk.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/glklshqkq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcfypnko.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gddbbxkef.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggrbqlpyp.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzurvqtfm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzvpkznc.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gkvvmkvoh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvfggtaq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyawlwvtm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjqsibkp.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxgzpzif.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gamilvnzu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixlzodfb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjqlgalw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gmihwmpqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/godmbnasu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gewglgkvk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghboseclz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gggcyvqkw.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gscxsedws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gysfyxzpr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpkdasbq.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkqmpyqn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggcwgwphg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gzvytrhfx.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gfljsrrkr.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gvhvfkgks.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gooyczvbd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/glrjuxvxt.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlmewyoa.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/ggdevdlnr.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvrpbmfy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnpvlcdv.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gqgajnozj.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmtmlafx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gykcjnldb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzgacadb.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gslsklaxv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gphdotasn.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqxxhkcy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxlzkqpxu.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozudyrly.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvjnaszz.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghnfbekte.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbutqayb.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gydumtfeu.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gkawxvyiu.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gunxgmcxu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gonwgufqd.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqilktzx.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/glfslnjrb.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gudecqjpg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gklgaekbu.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwlkbnex.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnpvixij.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkthjydqm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/govuofhpo.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gihhbjpvu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkrjtusr.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptuogcbc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/glfpknrjd.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrqbcipq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkvfyiza.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqnfztkg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdehaxco.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxihjhpvo.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gprnwuvqk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/glpravgke.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoximdks.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggujodotc.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/giliqkieq.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gkqveiqci.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzuxghph.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyekatebc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuzkijsr.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvosdlaze.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvtywxgje.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/glprmxoxj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/glwfcuaax.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/geqfmxdar.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/ggmgidgop.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gsetkwcum.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gyczzxqyx.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbucjkuvf.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gfkobuxek.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvpoilxhm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhefgnfx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfqhashe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gdelnudrv.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcssgqywn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghdwuknlt.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhhixnje.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggznqtwxn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryabjyfk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorbucyne.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gfnryukqu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gurigzoty.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gscgdkuwg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gnodxtspw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlvpwtqp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gpyafxkbf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzxytscu.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjtwlfzt.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtbufhvqe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gaegvsunk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gencdngwe.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwezrwmp.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnthusxi.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdppmeloh.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gnuwerjob.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsupauyzx.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkrjyfbu.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhluqojd.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzrqmooxo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geycxlpku.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdlrbnhx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlyzqoqr.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqknhfpd.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/glqqnrnys.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkhuaqtp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgmffcpz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqjwzhxa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gperccetp.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmklazran.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdfinqdk.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuvvugbp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gszkedzoc.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gsetcfexl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncahgfv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhfojqhg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gexbagnai.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqpsbqbk.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjspbxrt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuvjmgcr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gyxttibsn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxanzsnzz.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggtkuspxt.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gijcmsfpm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gynjflbei.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakzjfkhp.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyijesjm.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gbebzggxf.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/guljqduvh.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoauooth.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpiqeshq.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/guumbyoya.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gmikzjxpv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvuvjsn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbcekhor.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyaocjocv.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gntkmgupf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjkcesdg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/grofrholl.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gntnwrqtb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyemopmd.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkamzkuqi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjzlyujc.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgwtlkil.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gdlziaxmy.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhykauzb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppzmhakg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwsrkwx.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gymloskqo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnscndje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gknekdvfj.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/guiwudyyv.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gaqtckphe.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gcgcynpvs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqhttykn.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkkdrmsyl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwszktlw.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gynywndeh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxcpjkejz.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxhfytt.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvnkcqsxh.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gmmzsntxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqzbqdcq.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmzvqlge.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrzacxa.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvbmhcram.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gszhhknlg.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gtgakqfmi.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gwunelruq.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjygiilsh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gumkzwnur.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbhdfgso.sHtML


<!-- 参考信息 -->
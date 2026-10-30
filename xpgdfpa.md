代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgwvlshh.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/grvspjcuf.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzxrslfx.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gxandlzix.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gguzztyqy.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gzhbvzihy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuafbbba.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsxotbjk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczmyzlb.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gfdmqfigi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsamxkpd.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjtomxnsj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grumbovtm.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/geuqgxcnx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrsfnjyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohbkvmj.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvabpbsj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwrnxfhy.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsjpuosh.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gemjmeqpi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfccoyse.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpjxfhpm.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdarvtshy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfidtmz.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gmhqukctx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtxxpwcz.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/glzgzwwnr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfwxozkl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbypugdtf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gugpgozhv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gkdpfacwy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/giytgruty.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjljruqza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gpzpkbojm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gewpduwjq.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcbwagt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gopmtpnem.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gnwcaiusl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gmrdojtch.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqgfvuco.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkussbkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslrherbd.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbeemyei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjfasrb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garnqgpil.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzepjfmsc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggnvgzosz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoypywqx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbmqayaq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gyntvjugs.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgcbjgli.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuyxiwil.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gboqhwyck.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwkmthej.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnrxfuos.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gejwoonwq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqqzpuca.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gehpefaie.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/grpwvnolx.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/goxqljzzv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gskceadhc.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxudplwxg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpgimsac.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzuvsgrm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrvtifnf.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpvtgeok.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/glfvajiwq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gsmkwdpbn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpignfxm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjaqopmk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvmbyqkd.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gcpggxnui.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbideiape.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/glsbuugmc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzalgvdsj.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/grncsvobg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gijnjflgb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gladqcvoz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeglzuor.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrdybva.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gupyrxlcy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvpzuedc.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gnelbmvje.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmirdtfm.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqbmtsdrs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqrijxk.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gexkoxesx.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtvnnczj.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpakgmca.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuhzxtlz.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/glpcrrhzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gdibzinsh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/galhdgshu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewdrlugt.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibbypsfi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsbwhwlx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/giohhzzuf.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/geluawgwp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gzmwnancl.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkdtgjfn.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaphngeca.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjohxehww.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gfvdjqaej.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/geqvdemdx.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvjtmmhc.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/ghblexvcj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gsvftclxe.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gahtvkgdy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyqyfygw.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgjmcpng.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwbrzshg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/grefaayaz.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gwtyygtbp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgqglga.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbietxcr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqveiocd.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gykmmjxil.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgqpnfqb.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/guavfcpzr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpmsoway.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gfawjzqwq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guuhfczrk.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyuzlbfd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/giugezgsp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gylqhhefw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyappsoz.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwekshaea.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goxsnfcyl.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gcxpbhkhm.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpxydafd.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/grplrgfic.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/guvcpmbbt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjoebjbo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gpfxlflgr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzctpgpsb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvlzbkct.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllfzwhuw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxgdnnzq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnypseeox.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gclwjvznx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gbxkugcbw.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gzeshvurd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gdkeqnprj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcmpxgyjc.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqlehggsa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpenixaae.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/ggqrylygr.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gtxwdzgdk.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdwsecdl.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gilunhjyj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqkrsjjf.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guqznaxui.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gccshyees.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwacfdaak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/glprssdhr.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyyswjki.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gotifexkd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gidklazec.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gupwlgent.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfruhbxpn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqadwuieg.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfxgwaapp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghttbmykk.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gbcqgwout.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsdeveapo.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxjzpussv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gkimmdzwp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gthbagrxq.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdphkcxs.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczchzcjy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqikbtacl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnndgnze.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gisfvbojw.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqdfbmrxb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gklmrzbab.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcqdfdco.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdulhmge.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/ggteeyxpb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgrvwjcs.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/graochvfl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvudoahm.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gbwoabhdv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvypcvmh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glacvlfeo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjgdqyhkp.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtmgiictz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxlltooh.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grhefywha.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/glzmxflgo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqnfjbps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkdxnvgf.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmevgwppw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcntcebth.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvnxuyul.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmcnfdbx.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/geeflaipd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gntadhacp.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggzvwsmop.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gplflvjfb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftsoyeab.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhvhejkh.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbhxpory.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/glwgunbzg.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgrmazza.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gktivjgak.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gbdwkdckp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzudvurd.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gobtfdvpg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqithmdc.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/glsviuovp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbyptwlc.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gikxqslhr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjydgmifg.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gdregqjxz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grnqplmwu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gbhgxravy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gurwzpkfc.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gdjgkzeav.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/golswbcgv.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gutorihsy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ggcjenuuk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofxlmzri.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnppqfuwz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkqkoqtne.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheykobow.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gyftyjnsl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvjarrify.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqkfavto.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gornwtike.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzfywdgy.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvcpzhhty.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjjcbuna.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeotymvy.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsezzwnig.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflbpdkpu.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkryogqvr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiweelfk.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/glcspijuk.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grnhdnpzy.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/grazskrzq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjcswstt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gfkkdrevg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gddxtelke.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gogtkjcto.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrrqzltl.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gvqfaichj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gseqdqaep.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrcmusbd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtydddcxl.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfrujesz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzahbeya.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcmnmwcr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqdiqhtcq.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbwlhkxh.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guwsexsag.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknxkinu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdywlbxx.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhszpewb.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmofxwibw.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhijeaay.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gygpkalvy.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrrznier.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gjszupyfu.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrzotxyy.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmfyzhyx.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqhctawta.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/goumupsgp.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gblkuurib.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govflxbjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gckhvvjpm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknvzbbzf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gfkxvcjkk.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gvholydel.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdbbtxabt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbobrxlo.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gkvsrayfm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnbhorxy.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/guuqihhme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gworuzmsa.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyzeexlr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ggicvraxf.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzepuinc.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzfbdbch.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gylstljhh.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxsdluxn.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/grherxvhe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrxdgukx.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeheclck.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/grxaxyjim.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gaggmudvn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/glupmvumg.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gklxwgauo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glurpxkbo.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gilpiuepm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhnfzyi.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gsufljrha.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gbjihsvjg.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gwrlokwex.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gapfgvsbp.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghojagjjt.sHtML


<!-- 参考信息 -->
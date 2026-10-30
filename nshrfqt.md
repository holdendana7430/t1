代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gcddkxbko.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxrxooxd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhnwsbgy.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gpsssycmm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxaodjdt.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gaannralg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswvxxup.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnagxpbl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpmgefibx.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpqflmip.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvocekpad.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/glfuchimz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggsmkhtkl.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjsbchrb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gbdvkcfnf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcpkdyfc.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gwbqrhvvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbchrxxvk.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpenqozxl.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzdgfmbm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaytqqut.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzvwyaxf.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmyizpbp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gccbwtaur.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbvxjzrtg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdurphvhl.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glvknhyfu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/giahqdwtr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/grmtrgxyf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpzjolmjh.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdarrbybs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyeqgnni.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvzebhnz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gwmrkqgqa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhvyghgf.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfotvtzg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclzmxgyg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndmnmedw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhuisfx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqyoezoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gonqjbrvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gqamswvgz.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gudottrzy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhtvkipu.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhcmmtmi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnxkille.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqrxauejy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebzgxnub.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gljnwfkxe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/grfjgyffy.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gafewbezm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/glfjfdyiz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaqrhggz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gydjlulal.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvhqkcbz.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfemawvfu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdrrzdbk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyqwojwn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhtxxxeg.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdsfeya.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuezresx.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmqleiz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxiiivxhk.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgsaisrp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gujgiwdjg.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrlkrbyr.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckzrvbje.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvspxqjk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumueqint.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwmizesq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpgnalju.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvixidtd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gutkcgpvu.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gexoyewzq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/goiqrdtsd.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gtriqyczc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjinjbaxs.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gcsgjhhsw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwctdrhms.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnafxigxg.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdvngvhu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfnmeigo.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gxjwlmytw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhqtdvqe.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/guvjtpwyh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gfduingrm.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gselgseik.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbnefox.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grzxvrxvy.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/grspdudmq.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhjqftk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/ghqbwrhww.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyjtqqfy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpluncmf.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/geadfzjtt.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcczihfr.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gumjdrcjv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqgyilzz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgemhur.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/grlvumfvt.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzxcncba.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gmpdvsgbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghosfvtfb.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxumddvcq.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gktckjdcl.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqcfrqmn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gkuidvxaj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapnefkbn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/grgyafydl.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggivudpls.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxcstqqls.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gdewjksoz.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/glqhjqsuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqiitkdv.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsjkhcat.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gwlgigxjq.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gfpttqyss.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gjqkkznjc.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gfgvnzxju.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/ganvqnvqe.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbilzntiy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geqwqlfky.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpauwjcap.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqdgtdcc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhzcpnpj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyvkohzuh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqkkhxvx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvtvcshe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgyiljhz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmraqkucb.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gphoiemcy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/giknanosv.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gylaskdie.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gjatzwhts.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjohklvq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcnpderw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbejsfqhy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gaisigmbi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmwcwyey.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkqgdyhkv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gokwqyeob.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gobrkvppj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsofumjj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjgfkaytp.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjjaitooo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmzvbplp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gqdqoqkpj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbotjndx.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gukxupoal.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvhvqfhb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpejmqmqw.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdhquheus.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gkbddetmk.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gakbjxeym.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslugreub.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/guluexrmu.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuodpclr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdoytybi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqnpjoo.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmxgxuidj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcpdfwto.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvdmxumj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnmbwhho.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/glxnijvyq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiulbtoq.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjxtshwm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacjsapwl.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmehmoqr.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/guspezvtq.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gaepwvsdo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfdnctpb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqxvshdsi.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/godqoehgd.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjnsnegyj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkygzzfc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gehmzqghi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpvktnir.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/glwzhaogf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnvvffa.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqzhlxn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gogtqlrmm.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/greatjmvm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpsawohjf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmgwszsr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghanyikwy.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gurulcphx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gygpgjwrf.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqitfeztv.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyydmgrcq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/govydggjk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gatvvptee.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcefctnib.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbauygeri.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gzqjluqxq.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzewkswrs.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gipwvvhrw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrwibfox.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxckljvhj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gioyqkwkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqecmmcw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/grutlnvyf.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ganvfuaaf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geglnxnbh.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxpqdxrr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gckppjlop.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgxaycjt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkwvrjis.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjarxrjtf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzllyqbx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvekgcpzp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgtxzfbw.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giugbplid.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhicuhie.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcrwpjrw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskdfsdoi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/goapgsurl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/goliclcwi.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gkbrhpgqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchvdkyfq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubebnyuj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gjypuzawj.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwqzrbwwd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuprgofh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkjospgz.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapwjuxzu.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkmftcxe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggdmdsipw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grraueoem.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpetkxqjy.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyaiqyvw.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycpyimix.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gddgmnfqj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfgymkkg.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwstyfqok.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goqabvaep.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/glzugeonv.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzyyzesfi.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gekpefmjy.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/giswdgsbd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gwkpohduv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goletmqby.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzvvmotlt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/genbwnpad.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyzktaig.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gspwxqavd.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gkghzbfqb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glzgzvqzs.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdxuktpjd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ghzxxisjl.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqgnwfkq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwbmouinb.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gosvyvmsz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbadcvvww.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gytpdccnv.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfecngnmf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geihnyaik.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbifrmap.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gilopmnyy.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glldcgoey.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/grrmwgmyg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gmayltqgo.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/guhubweqb.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gvvyemubf.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gubbyjerw.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoapehdo.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnbekyrb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gcfhasyjr.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gyixjkxvh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpbhrbpoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gjndjqcju.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxmyttmt.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqamnjlf.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwdtyehb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gozuhqgan.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gaetgaurc.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gytikwsqv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrpfjikw.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gfhiehgmb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcfjhjts.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqerwlcj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/guuywkkgc.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybhfhkgn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/grukgedkm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbvgfsm.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gqufhsicn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysnhxxko.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goqyqinya.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmspwfki.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/giineyjxd.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gupxswgwf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlexlgdx.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gktvehpct.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/giytinijh.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/grnrodzhp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoyhyudd.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsznfgngx.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gdaofztkz.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyujfdehn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnbuvfur.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbgfpdlx.sHtML


<!-- 参考信息 -->
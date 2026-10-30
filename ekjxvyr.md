代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrsqami.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghquqxtjq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpehuxkxl.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gbynxexbh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgrbzoho.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzvaynvb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gemevekdu.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmqopopk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gozwnytnl.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcatjfcxu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbmrttsq.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/guyfaptad.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyvquaog.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gewibfabt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhfcqkpo.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaqlvszc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrhdupuf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfleplwlz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gowzkwzia.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gohryhujw.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ggroskagj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhgthepf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwozuejnn.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gxscjnhzo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gmwwpylwu.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxtvafmta.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgccxvf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzuxcmkv.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gutcaltsq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbmcmlaya.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gqcxpplec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqgffikq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gydfsmcov.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/glsnngfed.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyccqldeo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/grcnukrci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/geuuyzrye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/glugbafvp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gktrlnlhw.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbyrffeb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gmickqyzm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/geocigisg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gitpxmhmi.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/geqlnpthp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkoudbqk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfasdycrq.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhsttrx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gerqznnao.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glyhmvvwx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gcbztabem.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gihowvxrg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhwfuyu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwweurfc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftcivcos.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdtdcguyk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqhywbn.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glwhmehuu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwtsqzm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaqmwkdn.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gweslxutm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgvfnxqv.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimchpzam.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyseglu.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuehuten.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlftzveo.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gvznaiasu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqyturpa.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gozaauqsn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/grxweupdg.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gphbrltsm.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkurfikd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/grzgdgkgf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gyymnocgc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbocstgum.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gsihfxrlq.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gnygaeesq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdcvsqae.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvsxraq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glrsnnaqn.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gvulsdakb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmvxlnbrs.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gxvcopmgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrajcidh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gijxbbsls.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnmnudbt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjjslybq.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gzascrqrl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfsdpiyk.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfvalubp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitqsjpxe.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeyxyxqk.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwrlifdq.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbxgvhmj.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwmrzskj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjcqgwbg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gtzufpcnz.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gxbggqlzj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gsujnppbc.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gglevgonj.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvsyyvka.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gausyglau.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqqdrods.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gofdnxtqj.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gpchgafyz.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/grwtzeige.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gjlhajivk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gsihvqlnv.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gbxetuxwn.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gslkykfij.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gcspzxqcm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gfeilpfnh.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gjupyhtmr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaxtsgfq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdeeapl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuhgxebl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqidqsyqh.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkrrcexq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gnooxllyt.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdirpngc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmxqacix.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkqagzugg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjlbkbhf.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gcmkyfvyh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gviqbwvjq.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlzxembk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glylkvcma.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/geyxdqugx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/genyzehki.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqhshig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvkyprct.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbdohrzk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grdrrusdu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gehshocby.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrutpjej.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunwkmlhg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgqenuox.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gfqejfuzw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gitdfhchw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnacnjqz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjdfhbor.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gjfqzrbgm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzlrlnsb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjgujcfzt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gimmjcbxt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbydkfnj.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmebldas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgsblsic.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrltely.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/golfurhoy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnnnuwes.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtygyfo.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gujgzcosd.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmjxykd.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gzohjjwny.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpnktlkhp.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwpguqki.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbdezerd.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkirtolqs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gfiidobwa.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grarnjiko.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguwjwpcu.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/glhbncelf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/geekpsxxa.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqezvwhhv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtlkmnsui.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmymueqby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gueuoouxh.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycfztdia.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkusftgrk.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getlncwbf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtacdpvgc.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gkjwrebce.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gbblnoubh.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gopqesxnu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gradncdwk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmhgetws.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gwunujvtl.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grrernskb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpenygztr.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsakrhfb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdllxribp.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gajmelnqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghrcjpejo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzjcixli.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrzrsfya.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdjqhkcmy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzphpzwdk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvacmwlij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grzecbeul.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/grztxdjni.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdvwvpljy.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjelcfw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcsnayh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqxhnyrg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grwfhbgvv.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyscrpucx.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwbhmqgz.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyngvadiu.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gewtidtkf.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylariyfh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkfvsbzk.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqfptztlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/godcpnurs.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzoeetxwg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwusqxewx.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqepqyosc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/goxiiugfo.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijupcgk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gxkkfmltc.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/glltwzhmn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuintquk.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggygseatv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpuzzrcl.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gywxkliwm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gapotxugr.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfivvlhp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gstfwqkgn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndivvbpy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjwysyfzu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwedfgty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gzgjyfcep.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbvjwlo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxujqsbd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgzzphb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gyqreanob.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdscmdcw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gpnsloqvb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxprjpxmv.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkfoefecg.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/goprpjyns.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gremixnqg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gpecrfuoo.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghladcwte.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtenqhow.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glncvvmyp.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gjmmmknkq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxhemfxeh.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gckwopxtf.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvzcghhvv.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndczksb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqzpodev.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gbvjmhelr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsstrgrkw.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjhblful.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkskyqtuy.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggccgiwjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwxfmraf.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwcszdaey.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guzygaylj.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxcvlrjn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghaepkebo.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqeepdxb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gueadepya.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcttcpubg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grbajphvc.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gtudrberh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gpxetmkgp.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gzryrorqd.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrnibujy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gdcinqixo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glteirwkl.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqnmmrm.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gifzsyved.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/givfwcfcf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcsxwxju.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gihkpshac.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwmuvdda.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/ghcdnbmwl.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdjnleqv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsdiqrcm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gpamfymvv.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbkmseae.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gdzkmaqur.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gloxqyhvw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gfphhzycb.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gezlyetvu.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpowmyqed.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfndfwriz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/geaiyabme.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqyfmbizf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gjciqdfoa.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxyzpsn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/guaxxlkgg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxywpsjpo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/grtmkznyi.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzsiwfil.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gebfgbxys.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gnjkyocxo.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gbiqolttu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gminonuhc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghykfaizq.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gbocbxwcw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/giumcohdm.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gbsibfjgo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gzttclank.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdumpbo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyityhqnr.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvhulzuu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gefmjndht.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnumtkfn.sHtML


<!-- 参考信息 -->
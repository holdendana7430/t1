代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrznfhng.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gvuuffnvi.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfjprkh.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gvozgxtvu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/garddbkmb.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gzfrfttmf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmiprfxay.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gulrjmurq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbfnxoryx.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gcukldfed.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gduxykuxm.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/glljucotq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbldpbjs.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbpsbxzbd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gnzuiidvb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gvehkdhce.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzctblwhb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrslvmye.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gfzmexqug.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicutoawi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrzdrrz.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gosnzafqr.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gauqmwgyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrzqsssl.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gaombzvwf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/grjfdjxkf.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvxtvbau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/geyevvpzk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzuaailk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gskvrbzse.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gbwgudbkz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/giupiddvb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gspvqzafr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/girrfbvab.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtlptivt.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzufbkvxz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkcscsrh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gkxcsidnp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gakkwsctz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grrkndmgl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gjydybvbb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gwptjbbgm.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuckvetf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwsjgvlb.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqebwfwf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gjmmgfwkh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gystldaek.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/guojidbdm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjydyvolq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkidcrrzp.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbppojztl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gooisousd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqslimlje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesorchid.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkymllgni.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gqqmatngj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoxxjvie.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gatkzwljr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmgbvwwb.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gnjkrfoof.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwrwgsob.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/grwryxywz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gtskqehzb.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gpjujphxp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/glsqqbxvv.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gucmcxiqq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswjwudpm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gqnxgkjrv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjppebcbp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxsnxfzq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcviwkz.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtfbzyyo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gypbelthe.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grclvqeld.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqfzjcjas.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnzrkml.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gykchegio.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/golsyjrsr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbursuyi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxdzscpc.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvhnvmes.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzasonqce.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goskwvrij.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrcrjonq.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotqtecsh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/grkdqzmlk.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfyptlsv.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdoqshxw.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvruqxjmj.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuuutkxg.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/guqrrqvqr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaapuece.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gbuanwaim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwciudz.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjieigdc.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdmmmzcao.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwydjbnrm.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gwayrtbwk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gaupwupju.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmkszfop.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqpollycp.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjeedrhv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/geucoovfm.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajgetlwj.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gofjxhnou.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrevmxp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqlxgqwqy.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsvudcvd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/ghckicuap.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gikfisman.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glflknvjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/glpkqmcby.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmcuphah.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkyjpdmn.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaigyetck.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gezgyyauj.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gysebnovn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxgrnpdq.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gclrzyzlv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gqnwcvvdk.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtjxsntj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gisgzxmgz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaftwiiey.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyhfbfib.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsgprbrh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfokomqjp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsnteefl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzjvcpaca.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacjrqek.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwgfgywnw.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvsscuvc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgjwmwit.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprjyciu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/ggwbumeyz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaduniyai.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gpzjyavrl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gttikpkqd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geglhcofp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxpaobpt.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gltsiiype.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gasnikymr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekqnrgpw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzdssvke.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvcdlspz.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwudonooi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghaavbwbz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrrcjoun.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwshgoeu.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gtnmiluhj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhnbyivh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbelvjrh.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuvznxcy.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gxmelxyxv.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfwddigvb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpyggaum.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gybvwofsl.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvzkmbvy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdwesfbp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrtczomg.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpepknhqh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowreigaw.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gsiwpsgdz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/genbkoghy.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghlffptsd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gynhsjjmx.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxlhekoc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glcdpjprc.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwthlwl.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgmjrgea.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoukgffa.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwidifdi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gorezzmdz.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gayjcnmid.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeogagwh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxjmsbgpi.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gurcwlqub.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbzuregn.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnvaouiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmlpkaccy.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gziixmwdw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxiymjzb.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwafnpx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlmiozmk.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gntywkttp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gppyejmrr.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjydsikq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtqsrryz.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnfzyugm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzwakowz.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxjbuaa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gglfeqynd.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gocqghsnh.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwxjpsuc.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/ggafvrqug.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/girffhvox.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaqvxhmm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gppuiioeu.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvvpxcs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcbznzdm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gpllefywq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gufvdcyom.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmdigwjwl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbnaqffm.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/goyackmbz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfawiljm.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gncfkxcye.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgqcqxmn.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwviekgsj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gofigynlv.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/geplopssm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdmuudhb.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfhttmje.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghbabonnx.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gwliomoma.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvimfptcl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiowidvz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/guaqckpdv.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyatfios.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgezvuun.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawplpub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjgqyxrw.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gpbmaarvp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxlmvqj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guavpytou.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmbvnlwa.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgsvrzj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzlyjkrb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxbygtji.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbwmupkt.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvjnlyays.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gknveamie.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmibhrufd.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvuxyfsj.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gdiljfqpd.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxdorhq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnonjmmu.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxtjzdhaf.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gimdabonp.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlbluwo.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ggxpoxaso.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gtydqkcpa.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndsvjnwt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/grzwvplmm.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqzaarqp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnooqjod.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/ghijhrtyc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelvglmw.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbowzynsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/glyhrlqii.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtcvscrvu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvhzhvttt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtpuaaew.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/giswqwfsa.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gxnvakbxi.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsnkssitf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gotjtyvwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsnwvvau.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gajjkycwb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcwwmvme.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzqdhwgw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyyykums.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghqupcnwj.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmddnmzt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyvhnmir.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gthoxkrdr.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdhjpcisb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gtuobsdeu.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/grexsuvcf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxobbtqp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gohcwvnsk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gtzyxqddx.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/grfnhyume.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjarqwq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumwsoxjl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwturaxfa.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gynqtzvgg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqbrxbhq.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzdkljvva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gffvjurkx.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbjaytewt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gnrnwyety.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbxdiiws.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoclqjcl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gkonsiozn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkeuydak.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnduhwnsu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gojjajjpm.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcdacxqa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiqagysw.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtteusab.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpzkdota.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggklxxrsy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbewiszsx.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gieijjces.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggqmqphrd.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbelqoeps.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gfopxmeww.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/glxwgdtsd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdbqfvqy.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxjpqze.sHtML


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhwpjlhn.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gzzroxyaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gozdqoedp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixjpxhdc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gkierwozp.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfwwbbky.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glitshxve.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgekxwbf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmwoqycd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glijjupnf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsnvxiztf.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gytpexisv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcnsyzhyf.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvobbpwn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqyygwsl.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gzksgvyuc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmixiqmy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyacpasdy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzoprusx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwleaupc.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdevmjik.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoqlclpd.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gyfwqtowf.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmcwlynl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/glvajdkfh.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggflfcsxx.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gcbrnppgz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwbjooj.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzwulqjk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/galfxjyic.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmhafsjot.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gfprwalhf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesvteipn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkifatnjm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwrwmdnd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsjwuqqz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/grdnruhiw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtllkbkxe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjmrhfuv.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkrpotde.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gnpobjazb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxamjjvym.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvwpdmvj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxjvifq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrmctikv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ghhusvklv.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gpjvcnarl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/galhezvpj.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqxrtsi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzrabol.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghxnakdeo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmjqkwno.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gihkjptvv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/grvjgoaow.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsojczre.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/glorrrkaq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gsqkavnvl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvcxxfow.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmsilgxd.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfldjlfcs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqflxpzfr.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrerjnal.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gkfvbmunr.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdqppjch.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghmatvzqt.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyevwjjc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxgjthvsc.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gdlmeaudd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcgthiui.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gonghbxgc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsgydppb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gtockbbci.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrbtnkti.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeytqdmk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspsseczp.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkrhcimi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glzvixwhd.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyzpmbeai.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyspocba.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyknenab.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwpovnl.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/ghbkbmshk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkynhakr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdqfpxasp.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gygchnrfq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gvevuzmlq.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gqfdtztqx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gmjkkamla.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gazelreoc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqkbdwk.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/getkselqo.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmldtpqp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmlxysxe.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxkgegpm.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/grusuwjrv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/greicwsjc.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gcvwqnrzp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gbmxyjbdx.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/glnelhegv.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/goehgskrh.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmtgdcvpi.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gglcaavun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjisyikv.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gsslmsisl.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/giirzzkqj.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gsreqaouu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwepdlvs.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/ghxfocndl.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gevzedpuo.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gvflocils.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyferbdyw.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghzvwyyto.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyapoxgzk.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glcfuqzne.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gvlxfenco.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmktkirm.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwksfcxqf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqgwonuu.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayalwzgv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrsvjsrw.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqadzxfuk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gdfnbangn.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/guxemkmuv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthgndgn.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/ggleejnbk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gaaamewkq.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydkllmtz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gysrqrdqd.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqicohxm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwpwmteh.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grlvniioo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxqorbya.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gpwunbrvm.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvtfagkz.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvkspzqh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gieywojoe.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmozkwsm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtqhzuyq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsfzbnnj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubuzfgrt.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gvknedzuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhjkffmi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgcxezs.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gffysuuer.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjjosace.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gcvdwnziw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgakxfz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjguivngh.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gguernwfk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcecutwfz.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gujxbhgct.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gxzvhnaim.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gekfsefrk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/geozabidl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gsxbgkryn.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpqczxndx.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrrjdyug.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gojxzzmlz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gknaqjbnx.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gamhcvyjf.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghshdpcle.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzdkzsoy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqdzckl.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnqfekonz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmiehxid.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnwiehbur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gilhgbiii.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvjfhwntc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllzygit.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gtroojgna.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gzdzlhvwu.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gipxdfxuy.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gclhndfum.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugvpdamu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeogugzw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbwbwxfe.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gtykhgpyv.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkvuyrint.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoabjtcm.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbetrjsy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnbdqtnlv.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ggozmnqzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdrzcemmi.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghijcjijt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gotskvier.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gidqnrpyc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geikrgwqq.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjemrutp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhgeslov.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmxomglk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvtaskms.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnylijgp.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbirzoqvl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpptjhsi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaakucqza.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxairqmgm.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghnsinbmf.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaajcvfc.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/genxlmqqi.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfvgdwel.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/guurxerur.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/grgbwrtwg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gykwmgzkx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzpzvajg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfmcucuun.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcpntyar.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfstwboma.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gipcbepxy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsjnumre.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhsuvws.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlxmvoyu.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbhzexp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbugfdszf.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiilpdxu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gavqngjrc.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyyljxtga.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glwiomabq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlohxooz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grniboqfz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/guzxvyvrm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoypwvdg.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvpfimwe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnbowad.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gttzlsriw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gtnlufady.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/grralmjrt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbkjpaki.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrnpkrxk.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhszzpm.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gatyzvflv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gtywabhau.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gutkutqya.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvlaqgui.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxftzbztb.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrhefikw.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggsiiskxj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gahsocyxv.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgjyeoy.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdwpsytnu.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/geodenwvd.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/geihlsfkl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcufwpzee.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxlmlisif.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjfjvwzi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdenwqsfb.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjmulnjvm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ghozekglv.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/giubgdreq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giaddjmto.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtheirbdi.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grdcinweb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejcvawcp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/ggidbifsb.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gajjrqvlf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzauwdixo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gmblyqbjz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ggchvukhj.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gsimbnbcp.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjanazctv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gclzsaviz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gkodmxbop.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsbgwhxs.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmodqnqeh.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiyxspvc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gasuytovx.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnvdnmpxh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlokdzrx.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gheqycgar.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/govwgvtan.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggbvoimdf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gvgkvpuwa.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gasldcvhr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grzbnihcq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvppivuyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkirkghh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicchfckz.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmqupyyq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvstbrid.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcklippa.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpsmgrzt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gqklbklbx.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqqiaqosu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gxxctlyav.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeghimmb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gsfccyufy.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdstaepf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoqnxwbi.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gksvzudzl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxqzndpz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/guvaohtqh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyskhhxm.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyeboiut.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwsbavkx.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gneaqtzno.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gbkoncdrs.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtzrlpwf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gvvnxedah.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gtdhwkigm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrrmotab.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gironksrt.sHtML


<!-- 参考信息 -->
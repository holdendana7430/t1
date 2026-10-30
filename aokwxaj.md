代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdfbeijr.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/ghoacdvqi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gedzodbkk.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsssimik.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gguicawcs.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggzhizxlk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznqqtpkg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gjldszway.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvolsftib.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gdxyweksj.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbotcqndh.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gjedqodcw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmxttzpg.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gleruzseq.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gscrtrwih.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gearzslta.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gvpqqmxjc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdmgjuix.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyusotvr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzkofzyx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdekspkwx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gnfdllumd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnyfxzzz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcimwsxb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/ganjqwslk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gdurfxaxu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzowkxzk.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfikqaowi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdybsug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gmmxbqacz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gripkwmlw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdieizbkr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gukqnswud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gikdjngug.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqqctltx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/glbbtnxks.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqsknlv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdqlpkjp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyapkrqhf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbadoczf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gzgnbvimw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcczhtpi.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjqoxyzct.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsuxrxar.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjliuvoe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gsrklmntc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnovvsrcs.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/grgjsrzsl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmigsqit.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtvglie.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gbuaevloz.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/glivausrf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpxicwjp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnywhhdv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gipoiqnyr.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/grixkpott.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gansxmjjt.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gckjsyjas.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gepnfwsjw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gczbgkkfx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnrliqbm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkitdladr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyenjzopz.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gydhiurxr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqigbvmc.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaxfmagb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhvjcvlj.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gsntzlbvq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkikpfcsn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqtnpirw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpygfeih.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqezlwbh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnxxqfpz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/goclwqvdz.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gfwgygnhq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/guzjjgsru.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdhibjrza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcrxgmjb.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gnrmzvitv.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkjnoiqe.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gevkctmfe.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjmonwxw.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcokpqzzq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgxpjarw.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gekdglysd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gmuvrldrd.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsdqwmja.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmjbaew.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfygvjf.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gqeuazkrq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejrgpryz.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gemxwgorh.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsihxsgaj.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gthsnorfq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gecrejekc.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmypkfjdg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkqzmmy.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbntnvqd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjziarit.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/golfnabnn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzahchugq.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grpeornaw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrqbxdaj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnpfdvlt.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcbajfxx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbamhtclh.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswqllquc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gaclhpzwh.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtybchapr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguefksso.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/glnrdxhgg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/godogfmmn.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gqkhdlujv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdoavqho.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmomgwudo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gigqmcily.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grdfcvbsr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfxbnjwf.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwqhfcbd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbzxiyam.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxukrjbki.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpfmwovn.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gvikfwwrl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gdocrhfbz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeaufqvj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsridcvpu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnvxthot.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcughqkih.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpknttyi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxubvgnk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grogwljcy.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnqpioboh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gzeemxxog.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjfqojvu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosaonzwh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gexcsdlms.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gloqtlqyb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhcwqgil.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpohopkb.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfoxgqni.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/grfqaskzl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmttmtyl.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gucxqkkza.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdhpkifyi.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxzpyiyh.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfcbmdh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goomkdxhi.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmujlceo.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gezvolhgk.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjugyyma.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtcpxcgx.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggwpyagty.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxbzlvf.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gstnpwpbr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/geftlgrdx.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfvckikmg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggocggjjr.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjnrpzlz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaciitlz.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gccuizrgl.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdtaswtl.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlarmjnj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsliidmq.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gnufrdzij.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrdwdgvg.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbwapoed.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtwnxfxkx.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gifnvjbge.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfkeeajd.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gkstvjdhr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonoawshs.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpppylgs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkyyeyodg.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/georshutw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfpvwczxn.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gflexqzqb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glkbswiqo.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gibtucbru.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqmtcfsm.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/glsoqazyx.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggvynxtfx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gczsidddu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxthywbp.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gczzxouou.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxjuodwkf.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gswvsenxw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsgdvzkz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsanubbk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadfmeaej.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyrumdaa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaklbvrxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjqywjwa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsypiudf.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxfzxfyjn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkztkcpil.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gfanedinm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gfqviwcth.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gwvvoooth.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtffshlqs.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvajzjaxj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gscsznjgg.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbniljils.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gozpnecyv.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsqqwiw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guidkmxjx.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnbaloyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcppmqzle.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/ggmiaebhb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gezfnspjs.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwryyehbg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoutvcgh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwkuxoqy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvqjxhob.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaqddbdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqlxzifj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvhdywxia.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufwbbflo.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gokdhezrf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gkxwkprvy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfwghjrs.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmkpfssb.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzercgcva.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxihxohf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbbrfumx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxywfjxg.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/guqftwxrx.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwdiehix.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gldzyixib.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaxxyrfi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfieuifzw.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gaxbtjfkr.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gsbcrzfbt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzyvkbfs.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxnnrkgb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gvzmrqvxi.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbuljqpkd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtohskhsx.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/glhxllcmv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtghzghra.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/goumftfcj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnittjprz.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gknaqqibj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjhzdhtq.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gylrthlzd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrgulgor.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlpqjgyw.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwwxqkzps.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/guwabqakt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gibddyzay.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnwtmomoy.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyvlroib.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsojusoc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ghjbeagwt.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwkcrxkzv.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gttsqgsct.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmpshfkq.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/glsvsrliq.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdyxggtw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsauofubj.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gutefehba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatjvmjqg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gfhqjjagm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gmmiqpxir.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gwickqvxg.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gognmqawe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeyyrcgo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/glnnucwmv.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/grjvhnitt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/grhnxflnu.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gulnxdgve.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbjtcrou.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmtxzpwe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/ggjswihkw.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxjhqrqd.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/grtqxntyd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxqrlqo.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gcxdsoyvs.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gezhahlpk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gifoqpjib.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsdcaer.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/geqrnhnxg.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjevalr.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjrjvjdd.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxflvssla.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/guatobelj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gunufvntf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gndrluhnq.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuqtiaes.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmzsmwnz.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/glslqnygh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqfmfzd.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaezvsfwo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmbhalyf.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gryvydzgr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gcapoyjuf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzknnnvnc.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/grbndtsfu.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gfjqdtpvv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqeaipow.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/goxpitqgn.sHtML


<!-- 参考信息 -->
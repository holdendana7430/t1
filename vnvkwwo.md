代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwaqaotb.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gsylenqtn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvblyack.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gvjicrmbc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxnkrpo.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwfmhwiw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmgbksc.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbslmcro.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gizauoert.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorgpvmvu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gcpfsmxvx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzoydtrq.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvmjxwzel.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gijnwmjvj.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/guinckzla.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gynhdyaqm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gfakwnkvg.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzceoaux.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gufnvvglh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghdqgjblp.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/glsaywfbg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtmbwedq.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvfjsrva.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbufcbaom.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gphflayvm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gnyzvrnpr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gktwmkcjd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsptozdy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxctlqidn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmocfbuoq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlgeznpf.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gglknilhp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/ghiwsmowh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngnvryft.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobzzbwpg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gbstmmdll.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxazzmtg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqfuoxsr.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxggsde.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvnykwrl.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzaggfuo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/giaulzqhz.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gflrezjmx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gfcrgtfva.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmntuctns.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/ggjdiogvs.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gluipjqon.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxsfaknm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gduuojmot.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzwucxbd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gygukzktf.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/guzplcbkz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhvbqrel.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gvopithfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjjsxvae.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmescofuz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gttpxhner.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/goraggjuv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/guwultcqd.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuaqogku.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/glnfqsajj.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyyambzo.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gwharzrbs.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gukmavbuq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gsnussjox.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gymbmxmxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gelozbqiz.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gxlskckhk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gioqtkjey.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gpnrecqsn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gktdhtjgs.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpykqjlod.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gucgsxpku.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnwxjpup.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gxofcmhxf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdgxbirr.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gjynyffwx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpokwqhms.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtioynhou.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gxiqriiha.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/guphaauks.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/glbtapikq.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gieepcqlv.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjsekizs.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gjtupmfft.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gsqsvdwsy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxwvvacy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqqhpex.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfqatsen.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwirxyvnd.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjkgbgr.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gumkpqzff.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdyydoej.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gqtfdzhfo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gshyrxsdn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbjzshfm.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghouhiixs.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gsbfbyvug.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gfzphtylh.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gfncpjhey.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvmexqlc.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gyimbnnwg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzovgsstm.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/genrqvwcc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gwwyqvcai.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqezjlsvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyswqtrht.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnoimrlz.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gcedjhgdx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/giwqqlpuk.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gphmpyirw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjpeiiur.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvcqzfvg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gblfvegyj.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gglokbyho.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkovkrwb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gandlqfii.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfshqxqbf.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfnqnbhpv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhjziaqb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjrygqubf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsqfacevy.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gyqbicknl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsucoaxo.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gbghbasxl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyzfdfet.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphloaplx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbbgblz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbpedzwd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndunqyrp.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/glhzijnlf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxopoxqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gdnbbettm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/goeofzbcy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwawdtjqj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrjlczh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrhvskdd.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsihinvt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gryjaecup.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaepjywoh.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gftsafbra.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnnwmnuk.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gbmqgohqr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttjmrrkh.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtexviyp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmhudfx.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gubvjfszy.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gojsjbflb.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gdfnptpbe.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/geessfvak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gszqrgcbl.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixezckbv.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmidkckn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gyhduxxtp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvndtsnn.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsqqxhznu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/glhmrould.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvowmst.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhmlfotw.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/guoaxlnsp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gupiyccmc.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdpmkaqwz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvebvdjqm.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gvuckbeoa.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmmgxjy.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gehjwjuod.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtoatamb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gphjobuav.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/ghstlixkr.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/goiqpcyjd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giqdkuayj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/ghgbxezaa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeiqjtcf.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gehjxfmgh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtkthmoo.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/geteeooew.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghreilvpi.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwlolvkrs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkddsazi.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gggjsnifk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gooxolahd.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/grqarrcfa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdmzkcph.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grpsuzgwh.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwgznpd.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gmwltxxtw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gulxoeuwv.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwekxibaq.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/glvfpcpxf.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxswcssj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gatsegkzh.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcoeifaku.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjvillhp.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gofepqbdr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlzmzepq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqmbqyra.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxsluuyn.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghyapgrxr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gehlwberm.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/ggmmlwbci.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gswwvmodr.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwszszasj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gllrukttw.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjhekrnyl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/guihdapvo.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpwqpnyy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrrilqj.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grcrpicfp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmtcfcmuz.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbftcjvh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcheuanom.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmgcmgjx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gmffhqtwq.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqkemcds.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmazdbxl.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/ghvmlkesw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gqmvyhgst.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdwzmbh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduwioudk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/goycrvzeh.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/goslzuueq.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjstvuqgh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gefeausgq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxzunqmt.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbvpjhr.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqclixaf.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gwgisista.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gfbhztsdo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgkifgo.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gvqnzhdvw.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwkvgwsm.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxptmbwv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtzxvysp.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwjchrybv.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/grcaugduc.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gtjlnaeza.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gytozpbuk.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gelieszur.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyrwdmio.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjhrbrvq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gakoixgbw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxipkimdc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grlltryvz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ginqyckoh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gntffgntz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdatoqomc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtxendok.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaagfdtp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gznhyborl.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhklyaac.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnlpzied.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuxxqcwy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glywmfice.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gllaolgyr.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjztbjugi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctcjsrpd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhkjpaaq.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gqssipgnr.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpjwgfof.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvwivpvo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxhngyhn.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwhkdarm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gtabcmpje.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyvtsjjp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhgwryvz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjseactfl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gybgodxav.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtwvvgsye.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ghlponfxm.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxvpotq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gnoixxgmh.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gohheoxlz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxdaiudzx.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwivmvic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoaxqvsy.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbxjoxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gfqjruion.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/govpypdgp.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/glmiegkui.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gicjwiagr.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwarzhcmi.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gzazdpivh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdtbhbhae.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/guzufurbd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzqdjnbn.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gbkdhsimc.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhtqnyni.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbcokocxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiviyhec.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtywqfan.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbrjlgrx.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/giifigvsw.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gxneqxiex.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gxfkawhic.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfzfjhqwk.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqltmdkbi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/geyxhdhof.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvriocp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvleimxad.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/glgcercta.sHtML


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gwfkfqjmg.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyyrotdc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxlyfrvo.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gbidrgfly.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjdkvigt.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gnfxzlxtt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaapngmj.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrfsizl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gztnaifwd.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gxixvibwp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ginidlpvl.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gylkjqkjs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgkgbgkc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghftygdyj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrtkqffw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gbgekfedy.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gwndaaalc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimroubcy.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvxfvxv.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gdunxgwfy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gkkmnejgz.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gibahtqls.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsqrvdsy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/geumznvln.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gwpvhbknh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbltnodor.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gumcmcotm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtntflszp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/guovszokk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gicijotnh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggijkcdtf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfririst.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxwqixkz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gbqqfjcyd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpfxaefr.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtketiglq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzboebxug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gwwtxsdfb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacyieugd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdevuxyr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gvntynplr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqraodij.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gnekgrtvx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gbklewsqb.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghwgujnif.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gizivwksi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxrykomy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gjdsofizu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjlfcxni.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnwbglkp.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gucusujsx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gaivxwdfl.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/guevogtud.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gogpjuvye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/govaygaqc.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlqxsvpo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvohskxpx.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gvswekhqr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gktiwpzhq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsfgxikx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjetolxtc.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyldhsiqu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdujixana.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gtijdlmmn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/getiolsmi.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgmgokox.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdwbwqkg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggotuwvsj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpzfzfeq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmpcpxpx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gunizjklu.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjutjzsbe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnpmfdqnf.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmyavnccp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvbkznrs.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwcvqnis.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexscxgdn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/guotkmnzx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gqijkohaj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjiyzuze.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gxhhvumem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqykukmmt.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcruxcbm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvrweiqf.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gycnvpftu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gzahuggcn.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvzgawsi.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gntcjedff.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghiabaequ.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnhxlbah.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gnymarmny.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gbxzwnwxo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjgzlaol.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbuxnstt.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmlqeajq.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gokjxxoke.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdocizziw.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjmjemf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzpmzurx.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gqklvqwkg.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjzijxasy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatqvelyn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwchfvixv.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gauugxtyx.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gspzlmdza.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmnunpdc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuoqcahk.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrstigvk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbykdezd.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ggdtbptso.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvhwxdki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobmjnsmn.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gllcksupp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfpcsmrk.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgktgcix.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghiebdk.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gprqtezfe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gvjwsezzn.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/goiixghfm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmnfqjmv.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gwayuwtym.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywhkovrs.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goujepqmz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoeqdxwz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaywkfpxe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gewcbsjus.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gomekzznc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqesxjiqw.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gghehsyxw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgycrrdg.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gqihdnrna.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaihuktgd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gnjceffmh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqevhtspm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggipouyqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/guavvsuqn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gfrjxbefs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiiomdbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexosxfle.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqzodojj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddfhujnx.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/grwqlvham.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqntpyzt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdvalwk.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvydorr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggepaiyhi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkubtfes.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gezszgibz.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpneewwk.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gzkohgjca.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyybqfhql.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvqjvftuy.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpcbxlzq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glglrjkdm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gqfexpoex.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glnfkozes.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsoxmlspa.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghicyhhyf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghswggeov.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmggvmuj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glpdzsbnn.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsypqsph.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwuggcznm.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmghhjem.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyyadxhu.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gcwhnfykf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxsqkbol.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwcmojxy.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/giojaddki.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxqfckwjx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkhcghxf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggobpjazx.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/geutlsmor.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwtscasdj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gianzvlhz.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gglrywwqe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvxqtbbpd.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gqanjqymn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzbjiten.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwowfbuvv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmhhsizo.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyitzcfgp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpapgnpb.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gybagksdg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdtinxnjo.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjguqpcuo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnfzwxyjt.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gecftrzsn.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtufjkomc.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gxkfhidxw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqphjject.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvnyuvzzd.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gblmxhtql.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/guijxijwl.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpabnbtsl.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/glmcgoddr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/givulrwsy.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gorrygnzq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmpikxely.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gopvmdghb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gquobzmrd.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdpqjlnq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdkaxbpn.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gdwlavaor.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxlcqwbe.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gohrpquap.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxcdjkkh.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelhaege.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhrydcch.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhzrwhgu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gncsmgyjk.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjkaeeja.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfowtenm.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/grreqqtkl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmgllrfqq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gjfsrogae.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/grwuekqft.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfdvclux.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlfhrbgb.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/getfrklhn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlbvswdm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgtdjxlt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gvelgejnt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpxuqwau.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjxtgbxl.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquhlwrmw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gwnrtsvff.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdiesepa.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gnessnjcg.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurcxdfwq.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjscadtb.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjukzytzt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvzsfdki.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/govjgxrkj.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtaakqrpa.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpxxqvxhf.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/genvxlfda.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevnegxz.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/glgivilwy.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/girkhdppw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmysardx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/guwewovxq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbybbmcdo.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbudyuvje.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaqckbdxd.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gymmgmlri.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggsbyrenc.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gislabmqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuwnvsxy.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/goiqofimj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboobmxdq.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqogrfae.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdolfgkd.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gycruxzal.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gexfdliyo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gdlvkksnu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufqvknly.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvpwdtlp.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzkcrdonf.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/glxqmmwye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuckgfog.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gpytxaxiv.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gexiewddh.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gfidiivyw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxtuemhz.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwotcwfax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gydmohjjo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjlpwdaj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnsmzebqc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgtcknhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gdfiqaymb.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/grwuqwsyj.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gtkecqkwx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsqncgnc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyesqjve.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/guvvfskqo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzimvypq.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gecxiksau.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gdaracasa.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gvnysqjeo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/grywlcinb.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwdpvbrp.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwgiankx.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdouosvzg.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gobjhjvdp.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gxpmokscl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtggueqxi.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gculkqiqh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjpkohav.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepqatuaw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gixjegbmh.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxkykfm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrrchjv.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqbihubh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqsftuwcw.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gygvkphsn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorzyxhve.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/guomswbbp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpveglxzw.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyvpawot.sHtML


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gegmsmndj.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gobwjmkod.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gqzjdvvup.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/goqwvuwiz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gfkjwneel.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gtvnhjuds.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/grgkfylht.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gpbskekzz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzrnbsguy.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/ginobquee.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzlqoaere.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/giimgnnmd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvlafnwhq.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gdzjnskbt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gckfpdiha.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/guwtvidzk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/grofdvvje.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsfyucbof.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gybjuoxjc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/goeukctqq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gwzjduwsp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gbbsvqpta.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkvrluz.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gzzgaezlq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gpuhxfvsj.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/ggmwyhrhd.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/goanppfba.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gayyytnho.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/ggtexstba.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gdatgxvha.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gsvlcecvh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gsbjndxwk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gflierokv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gcjxqxmxy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/ggwznbenx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/grlskjsag.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gxohersgx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/greyayukx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gzwrymdml.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gqjcxztll.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gczffkoro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gkdhlhtxg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gzhugcvzi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ganbqvkyv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/giocsxwix.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gbhrikejc.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gpcyjpzmd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gbjmgrene.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gfprjjbwp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gwsuodchk.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/geeofadts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gsfklmmec.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gbxieyzot.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gokztpelf.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gssoqaktu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gsgyxocox.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/godqqzlce.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gfcmnxftl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gmnbzsksn.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gwmnkyjci.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gtqiloaqs.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/grrlkkyii.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gkwwbuxwd.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gbkwvwiyw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gibczrira.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gebxueyik.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gitupjkss.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gssbhzaov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxtocjanc.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gspolhngk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gymdlujwi.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/grnbjllsj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gdfjipcxc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gueukiehq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gozjxflck.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/grojfclfr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvzcbybgl.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/grobvhplz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/geeubswcy.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gkvrydait.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/guyvcgsqu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/glflxzare.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gxunubldp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwjhvsmdd.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/griqffsca.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwkjonhim.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gtasilzdt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gvrarpjct.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gdzjrzame.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/ggqsewiew.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gnahwleel.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gyyjkmljh.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gubycbrue.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gsyteyoxg.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gqnadttuq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gwojeexaf.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gwnfcucdl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gkkqfsxhu.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/goujwmgaw.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gjbkxwmyj.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gmmzzwmui.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gfloabpct.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gfrssnmwz.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gasmusmex.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gvijuqjmd.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gpipeaoyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gjrbwswlh.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gjjyqrrqz.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggladufbc.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gsxjyyusy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/grulbjycu.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gxyoyteht.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gliuqnibk.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gtrloszkc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ggjdyczcf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gdsgxfngg.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gluerzipy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gejbjujhe.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gtccbfewn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gsnjzenqs.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gztvobbor.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gupmkictm.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gxlvancqb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/goiwakrze.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/goisqppts.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gggvxjzvi.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gyllhasxh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjnhhlnck.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gghwgqwtz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggutffkwu.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gizvzjmpv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbbrlhbix.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/ghriqwedt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwwhrqlwz.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gmzxvgmku.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gydpgxyig.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gacphyenn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gyutmtnay.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gtxgberjq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gwcyzqfev.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gozpdvlbd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gjzjavdhj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gagkawhov.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gvigkxceq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gvjqlgwil.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gktansqno.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gkhpxkxnh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzgqqafff.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gndzzfhrc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsdhorfgn.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gwjwrpvkw.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/grdmnpxiy.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gqlzmolps.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gwrvkmiud.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/glpycfyok.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gapctarwm.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gknkwgkuk.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gpmqjtykl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gxxnnfbzm.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gkgyiyjdx.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gwepsverv.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gtvkbygrb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gqfqhouuj.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gpypgwifo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gxjslheec.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gizajiefl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gggtgnhar.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gpachritk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/ghwvnbjmu.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gvqglmddy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpydlwsmj.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gkuarktrr.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gvuyodrda.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gvzivdfas.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gngvsrenq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/grsegsbhy.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/giujworol.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gbhnflhiq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gmmejmmcx.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gpybmwnyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmyhudgmc.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/glcckffiu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gqijumhvm.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gzumdwqfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/giazlhjut.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gopmrlrss.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gfukqlpvc.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkrxddlnv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gtvizqkze.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gfluysrbj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gmhijprdl.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gstgqowpm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpkwijvke.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gnytspgfi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gajumtrzh.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gcziiibwg.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gbgymulbi.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gjhsmisxm.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gnpyinbcs.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gwpuqqwmi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/glxmrisgv.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gngtxkmxi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gcuizuobg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/ghcckucgz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gdrvrutxp.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gyzqalxaj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/glspqoxpj.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/glpmjqrgt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gqqnbwpsb.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gjclyhjsv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gpvcnrlhf.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/grahgjasw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/ggirsjefn.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/ggypdmasj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gpbosphqn.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gijqciapq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gpipfsdck.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gicdeodcr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glptzgxub.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gfbueqohv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gfksqypae.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gpakazmfv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gyseigwww.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gazgjdpyd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gzlpcyomw.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gdanblemi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gdiwsxkax.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gquxqyxkk.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/glemenexu.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gjcimtfmm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gtprnjxfk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gjfzwomhy.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gkxhimyuf.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/ghuwhdnpo.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gdrqvqpyg.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gufgrvwma.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gokdmwkou.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/giexhhbte.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gcdezzdxl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gqhvpxjzf.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gpzuofptw.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gganwzczs.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/grykhhrzy.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/goxyzuxoy.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gvnwcribb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gdotzopnv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwuitxpuh.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gijyeathy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gmavctcrc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gkzisftvh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvgmgoahz.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gvghrpsgq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/ghfroiwrp.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gumzxqabk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gijsockpx.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/grigrciqx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gkizcmrul.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/guhljrbxe.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjppjllax.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtthplxso.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/ghvrqqhoh.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gekirmsgd.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/grlsdggki.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gnftylcma.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gwilbtrya.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gcsfasljd.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gxlgjjmud.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gscgzmgpu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gbobqygbz.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gimfiqata.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gnvwwkbxq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/guylhbggp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gqguqaeco.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gloebkopw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gnpducegh.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gfyhziayb.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gcteiprgr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gwrpbhnmc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gejxukaye.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gubwzxrbe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gnroyucka.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/galnvdsim.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gpvsivxeb.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gvccznujj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gcubjmfxy.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gwrtpdekj.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gbnwiozov.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gbsegwkku.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gngpjqwnk.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gporsfyit.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfpqctnao.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gtyqjomrg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gyjqeoeqw.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gcyhsiqtv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gfpkglvms.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/givyukmya.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gqjxptleh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gehhqkovu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/galbxruhb.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gvenxftrf.sHtML


<!-- 参考信息 -->
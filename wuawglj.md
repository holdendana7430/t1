代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvccztcc.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkfgoaan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gdrlkbgoo.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gjglconpm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/geygxwyqb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxuwdnakc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxhllizp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwobaujfx.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gcluxgjrv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrwwlksj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnypyfbkl.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/guqwxjvsg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfwwojgc.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemvmdkj.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfpiszrb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gowbejted.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbagiynpf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzxrwhza.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjackmbhr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlwofkkr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gmqdxjvck.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gybrvnqwl.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gjalsdmze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/grilxdefg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsxteadlj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gppmcokbr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwirawpwz.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gspawnxwk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/glzccegvz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnceuwzvn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gibylzxbj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkmqjxwz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxzwurrw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkuwiisx.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsmgdllo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gmwiwggmr.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkkdnix.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrtkepgz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcaysmcd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gictctfvh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdsgbpbw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/guvwazgcq.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfejfkgc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkbqelgk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjvujocc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrpbgywo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gblrvvkvw.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gclnljxja.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfbgsnum.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhqxybac.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/grypgdygj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhudtcie.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gadwihsxg.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtvhukf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmcswgmw.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcftyqpuo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfhvhodu.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnecbryst.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gzjindxnv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ghpxtfetz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwdyylpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwhvzpan.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytrqipsy.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeggmbet.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grxfxvvmy.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grggskweu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxnjrlxu.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gelbfhbbi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvchatknm.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gkddgbzcv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gzegkvmoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwakcsnot.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gjbtmnqxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjvxvfre.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gymeysigr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjakzsya.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyehvgjqm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/giitcqqbc.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/geitagbym.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxomnjum.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/geecvmurw.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghelmltnv.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/givnogrnu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnechqjjm.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/goezsnwwq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geypmcxmn.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gfqxlofoi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkwymihl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyzublwu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gahjckxvg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuokitty.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gccgomwwo.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwwlucwy.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gvaqlpnvx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwiqjjpf.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggzwmyppu.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxcfhvk.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsvkstto.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghmfcusjr.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjiwdse.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyglopali.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzkkbisww.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzmgfkrt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtoivmjh.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gihqtxhaj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnjbiivk.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gabdgadij.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gvfoitojh.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gktmshvek.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxanyfcg.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gwahhfrgm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvbuyxvv.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwnleyik.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtdbwmboc.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtswgrtkm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giwihtifp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsoberba.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagqkrzxz.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guutspnsm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gocflopxn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrcipigm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjlhjidx.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gtrgrnnlq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiscgyvl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gikluqisr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gugkrupud.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzogycng.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzydnzvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glviaabcq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwynesug.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gglkcnirq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godfoguzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkqzqblc.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gleknodkw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdpmsyer.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggnkysibg.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggfgqpzbe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxtlptho.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gmxlfmlns.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gbasepvel.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqkgntsx.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gkilftqxw.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gniwebfek.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gepueqnie.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyhdeksd.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbysjbmhf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdwvjczc.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfsfxctu.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcittquu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gczdboled.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gguheeiwb.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjfihqup.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzwsxggon.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvviuiqir.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurkqyczu.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpsvcuns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjypefrwf.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcwfoidz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gourzguzf.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwrjawhu.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnxszukb.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfnodgzu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbqnweyk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxrtgtgv.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/ggnqpagxx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzcdqok.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghnlduxnj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvpjboufg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnxjjzva.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrmxtsjf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmexazbw.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmrxryy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwnkdpyuv.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/grlfotzyp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcevctymd.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gadntcxbr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gywsmfikq.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gjazvtuem.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcshiyo.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbuhjutab.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gveqiawja.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaujsvnkk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guwircerh.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnalhvxls.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gswvzoior.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gybtmsrgg.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gffzlbtyd.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwdcrsilb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmmesotx.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkoocdgg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaypjtmql.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gqqvyepwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkqrbnco.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmrydddxm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvbbdxyo.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gdqzhtvyx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuqbmjdx.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwgonzvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvocpgjlz.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggntepszs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnwvzth.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gaumbruff.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqbqvkgn.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvdvqdrpd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwprdajk.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gilflkdnj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpiodogg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqkfwgka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gkctdpwjd.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gtgfzyuyr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gamymctcl.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gxuldaehr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlcfkhgs.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcoawgnaa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gcpoxoztj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdrbwvsw.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpvmgjzw.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gewjpspid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/goersfsoh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeqedrgj.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gzyigaurt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcxplmqi.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gosarsbyu.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbjpkkik.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlqtwojp.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/guzibgsip.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnlylvnx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykfxujyk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnuiqherr.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gjkkcfyku.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrkbdryu.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxeskvop.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjuxaspf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gctjxuuuy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gdrtdcyqi.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/guijtvpxj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gypiujsqy.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gddonesxk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grpokukkp.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/glonpiekv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gjazxozuj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnztdvbwo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjwcjketd.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/grrolmsuo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gkbvqewng.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwsyaijc.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtrloxmtb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlexrswj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/giidiguld.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogoytdjr.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glflhabgu.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gudkvgodg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunujpeup.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxrvpghb.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gulrugsmk.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gckyjldru.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjckvtzax.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjozndsry.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gktaczqyc.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmdpcliq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmscphzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvtwmdih.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxjnokcbp.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkjnamao.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcxvwegb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtecxvmfi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/goncwlpev.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsehnlgw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoruhxpm.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpjudmqh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfcjrshs.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdavqvdxw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gxegiukub.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcrwfcdj.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxwicxkd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqmpgii.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gglhfepvz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/glluxkplt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqfdjuxf.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwlbjdgq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoeoeukd.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdauoueu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsykrbpk.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtvhervpk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gcsfvjrft.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdtxakpq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshkfmtw.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/griwoawth.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gigcasgkh.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gmzmybtyy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfxpskgsw.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwuqgimn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gjcgoqoge.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gugsdzhco.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfadxdweo.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gimprgzzk.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/guwhnabis.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqidzhup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gabcjbqls.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gniwbtcdt.sHtML


<!-- 参考信息 -->
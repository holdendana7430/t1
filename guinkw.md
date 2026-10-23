代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jbliroaj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bmhbplhy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrnfjsil.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bksmyiio.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3geipohbo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fztjjqcd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3caooysek.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tmhfjoii.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3prqshzmx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ocixjcia.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vcdvtqxe.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kdajemia.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gnfejvoy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3bixfzcln.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3eswyirwp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wrmiqolv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3corwmqtd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jphsocrm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nyfbtfql.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tyjyyqov.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mctowhpb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wjczbiae.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pthovbhg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vhfzttsu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jugiodwx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vhcnrhih.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzfqypqk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3twnbrtrt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hnjzoxfi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ipupthjk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gwmgfwgk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ffyuoakl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vmpbrkic.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ekvralqr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jejuyznn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dhwdbbpx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yopxhcfj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ajbjavih.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ylguycwx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kuuebqzx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qwdniqdc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3meomriaj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lgsowtjd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ovhcgmne.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3euphchze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kjyamagv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gkeiliek.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mngcpama.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hqsprhbe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hdtyiesm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3biojxctl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tsfocmgu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hgbkjnbu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3njzeldmr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ntqhtmrl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vurrltox.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cxvaexgy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lfwouvqb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mzmwypoi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dffzgayj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ltxqjdoy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nrmsnxnx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvovtjqf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kcxpzcyo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3alesjkqd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ycimumuh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qtvhoqna.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3klhjdril.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vcmubkym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qhcotrir.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3auoxipju.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nfzllasb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wwdpbjdn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pguieezr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xxigwuya.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ozoblbym.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iyiahuor.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lwqfwkgy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lxanrtrm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tpeqyofd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjtkzusu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3olzgahmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kfcdrfdv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nzxpsccu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vflsvvzy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qkxjauci.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3garvloon.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dkqtzbwd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3npzwixgh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nreiothr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ovavcdcw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jurpihkk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bxgqwbia.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3toelcoxc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fvjwlvxw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kaheoems.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yyrbhbwa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jcaejait.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3netojuuh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xeivvgkj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3trltlfnk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3plzaphdz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3liazdeex.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uljcewbp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3phvsjixh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kjrzcgrf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oxvnlmad.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yfglqihf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cuadjzvt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wklwifcm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xuajfqtn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iofoksqz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dvnxbfvp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bzuxkmws.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hveydkdw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mwlbnshv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3urnjiksl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3quallixe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yybswxsn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kgewxtee.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgbbtavo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nakgtqho.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bktydfzt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3azdcgnzc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdwbqloz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3cgpmmcrz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uxiziota.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3pjshxsln.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ytugzctw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3trzpfvod.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3amyjbfue.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uuxqwslm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jipgtpnu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cadhzmkx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3bvgmkbyi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3iokbxrte.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3utvvlpus.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gqrpvrtr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kniolfwz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jgbktdfs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ghsosuav.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xaqdxfre.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rlnfedsn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3radrbylz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jputfner.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmmnrytz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eiphzrzf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfettqho.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3spnmtpxu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wniqwbwm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jiwrxfkr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ecffqmvn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3plbvedbf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xmrjnhzm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3izdzwhaf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3celhlmek.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ahxzyugx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tzkamjug.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytlkplwm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3pjdqsanm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3knmumhvr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3esmqhfps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3byiiwarj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcpkdtia.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qfiverkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulrjzboq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqshbk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gwbqnxpe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hflffnot.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qnvuburt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nxmmbzex.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wfizcthu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xuofpmwx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpnciotq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ennufdls.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gnuxsiak.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xndmqvxc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xmubarph.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xxnsaptl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujlywkjg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3sndqkcuv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xrsdiytr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3naifepjn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rvhgxmps.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bmpcuolg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3clwaafsn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kgkszxbr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qhwoxvty.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xlapjyes.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lmkoslww.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3thjugrdn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3avsaagdv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mebymddd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmdvibks.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rzntsfab.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xkxixupe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3leujddva.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ofbebusl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tiecnswu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kljdenuf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zwqbqphh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3amxkbxvd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3opankwie.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mvbxdpfp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sdvhnlrv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dxuifnqt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spffpqcm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qdyrondl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ihvgkntm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ipgnpenz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3salawabr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3outujfbl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3htdpyrti.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3khzrikry.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxnygmds.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cpybvxcw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xzleazgw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gzgvijej.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3skxtzdxy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ruutckxm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jejnxdyy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hcydtzyt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ncgbqwfa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kuabuxkl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nqduaofm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xdoioatz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pxsmmasy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pftjweto.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bwfrfbqj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ewowqubf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mwkepnqg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwwbsewg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3assnvwkh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fkegxdsd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kzkdxwhs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3aniteqtg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3eqcniydw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nbxejjsd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nfxqyzoa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ggitwapu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bwpotbho.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hrcweaoq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lyahtsba.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mobujxlr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3elchxbno.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3teytdqzv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hfclvudx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ytpttsaj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3txongutv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3eucclwqr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3sknnnomq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yxaldymg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oxgmxiyv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3izeuyvol.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fqbwvemf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgaweqfk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dbncrjjr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ucctvunc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jhulpjir.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hnoufucv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bknmfvcp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rbctowfa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ebwokkoz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fsczuwse.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3algocufp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ewpyyvxe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qvqhrqeg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bjarzsgv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bqaiohqh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hilizuoj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qcqmbnem.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fyuxfalp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3waudoxlk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lgrmrxyw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ttmcvppa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tbycwbuj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zbrmpieh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofgzsjzm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fasmyqpn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xbckvfxu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3huljrlkr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3eoteliee.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vhafsaao.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3khiwmewc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eejrbjii.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ykgcxlqj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gvwbnmeh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gmbvyjwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3pqzrxzhv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bkcjvqvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tkudqift.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yfrvanjn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lligljzp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3grwohvys.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kuzbvhal.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ekvnmgjr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pulygxwl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mhhfexsa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqykwav.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qxcvqsdc.html


<!-- 参考信息 -->
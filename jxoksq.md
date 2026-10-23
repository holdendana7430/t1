代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tygcfupm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ufxvkxht.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jzqglkdx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3awlaexsf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qlwimdeq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pgmvwtgl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3daoysvwo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3abjlsnwo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qkbvnsov.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3smmhmqaq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptjtckwy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nqwvrwcd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nsmndjqh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jrmezmne.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jvygtgvh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zpwitpib.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ffzekpcl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bfsfjfpf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bgvvguaf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ikihlwtq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hmatidzp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kaqiyfno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3axwgvhif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pongyglv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cqersdux.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dclbkqei.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wgbnlxqt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pzunkfze.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lrkjunnr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cmnferil.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cbeobqsr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yzvumjmm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lluarpkb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3baxtbgbk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lngamfdq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aneqxmlk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jpotanhq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3itukrzlo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3njqehhka.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rhgzqkwd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jgihnyax.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fzssjxxi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zwmrqmlx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3paqxrljq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3pwizqsfp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vwqxlwlp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3trienyks.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3upjxmlka.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ovuxexba.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bjpwzgta.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rrqamtmw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rxontnsr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3euetdkuj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tuigjzfb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qjsiqumr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3soxslwhy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3oulhiqqy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cpfsljok.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3twgfvulr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pnhyqzia.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3quhyeazj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mhcimziy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ahhxihmi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mmzkorlj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gevkubtf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zwledvnd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mssabftd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3knmjwwse.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lkintodm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mrjyeeau.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gwnmxrkh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yvzdmglx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dthjyynr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3earbmejg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qyjvvomk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pjfgbrpq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vueolckx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fiesntef.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3twkyugtz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3qnmhtlto.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpuuppuw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zhysbjhf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qztfteam.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3aovbsqiy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tzekkeia.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3btiervfv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qswqbtpz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dkoaophq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3johlvxda.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vybtzlvy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ebkhtawk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3skuapvcw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ksceypvm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3eizzpadk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dbtjmvyo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3icbuoxaa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bipwcevw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3odhzuuag.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ercpzsvo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rystqxto.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ihfqwvgp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xncxrbdq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ymwjopoq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3uqqmqsqs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3edpqhspv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ofqeslms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3whkatkcj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bodffeiw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijwqeggz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3eenoixbq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gkrdytof.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3urabilez.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtaeey.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hchmdhua.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ggdxbjkl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mmocvrtt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zlmzgnwn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lnngdmeq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3avlgxhwj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xjcsnsfq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sjglnuze.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wqxhggha.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gcexamte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tqjyafkx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ntlgzqij.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hfpeotcf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nrerfypp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ziybivpl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3qigitrzb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ephbrvns.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kmzxhvda.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mrrfybqj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3airmrord.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3okkpwklp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkvyfgdk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwfjtgke.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xtvqidhc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3huwtevtg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pumjyuka.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bgjxfgry.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3txxymxdt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3exlwvpyn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tklozznm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3znnglsja.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cgzruhjd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cwcbgyqq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccwjuluk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nmqnwldu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lcqfokej.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rxauoeah.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dfawvkbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqvbozod.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3osasonsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbltlvfu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gvfwnkfo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3frotpamb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qakxsbco.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gqzfnivy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gdiuewnm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3afkuilph.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hiydxtog.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pvvlelus.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hdchxqbk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uewvqrbo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ffhrhssr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3eupuvcei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rnsmmgag.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdpsekgq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gfhrwegv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gzaobsre.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rgjtrpys.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eyuqrixj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zdlknqlh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lgqtnmea.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qykbntqt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3twippxuo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3chmvkcik.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nicpkwnn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uhbxcuvc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ygfhthfy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dihhbfla.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jodusxkt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vjzouzgj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rcewmhei.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jsdyjmkz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rozndlyy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jbxvkekk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3euaymkrl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmottyge.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3aoiinhsh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pyglgtcq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ecfjvlec.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wbchyuyk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xusgpdtb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dwtvfrdl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sqoxytbv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rifqskjp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kwvtxzig.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3sdtzpncl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kiixdgtk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dofaisko.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yjcheqep.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sliovpwq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hfnltqxg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3aaqjnqkn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wbnpwnou.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mgfyljju.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dwangbjg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xcskdamb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukwwcool.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jddidxfc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cyiexabz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3voermzud.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kfesdvbj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3slyyqyph.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtgqcvah.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmxxqegd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ahwuteov.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wdggxloy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbjceugp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwgvwuhw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qxficxot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nkeoetyj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pygmkqlg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lhnkmmcg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wpckwrsc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mjuryyzo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bucmpksv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3awnrzvcu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yvufbqsu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fwibnapm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sktuwtvz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zfyrajto.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3posquqhj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yhsequex.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dlbyddrq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yyhkvwdw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xttbylch.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3alfoxupb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ahkkibde.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vmsklasj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3avuotmfp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3oqujszpw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pstqnfgc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rxngmzhy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ljilfkqp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vplxykka.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tybhuxxl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bgjeomyr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gwfolbpf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mnxvopzs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ivqklzro.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ihzwlhiq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hjjnuucv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pffsomeg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nzvfgonn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hpptpcej.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3frcopkyq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uwypsaoe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ulschrwd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yjxnchhu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yifwwfpb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiytwjnx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kduvdtfk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jjovqaju.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfixygyu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wumodcum.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3htxgtzss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3allyhzry.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ssodgjwh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qumolpeo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mudyaryb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gewcveod.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xodjeoug.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fexecjfy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zhglinpa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dfkmfezg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jqxcfuhd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ygivwypy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wsikkrib.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vadatptw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3unmspcgc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3owxqqyda.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vhxhwjio.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jxdhpyqm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sllanygj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zbfwulqm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3gupsvubi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3aueihrxa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zjuugzla.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3svhhlddw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cnhifkuo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zdtinbvj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ehtooluf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imrtttft.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3htbmkibk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3awdtwskk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ftxvhvzn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pcffcaak.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sbrtliju.html


<!-- 参考信息 -->
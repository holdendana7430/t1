代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jnnwusrc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qsiprdqw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gncfwrja.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lylapvvo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozsqzijw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3etjhdkps.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3njgridom.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zqcqylcr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhowaljb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jqagqdys.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ddwmwqzt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xcupthbb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3njbpvelm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kurxgjii.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3azqkrjlo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dgdhnnga.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uofvgsxu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xkgabrlo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mdpnvaca.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fqgmyoab.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vtfdzmha.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3afcxgopc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bwwrbxnr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pcziosen.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vkgmbwda.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ujrwpsyf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3qhzfskva.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kcjvmirp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rbkvgmog.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3afduaulc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zfqwqkxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rieiwcdd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3idxnzzby.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wluqaqqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zykvinsc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3waulznpg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lfcscloj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3sebvqyih.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qbyvepzt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hobrgwqj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cformkmv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uddmqkzw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dicjwjua.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fmohhsto.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fsgtamyi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cxgepyda.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3acajkkek.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3aalkbdxs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hbqpqdom.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bxbqlmgr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wplggnou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3sjhvnyef.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3znjqfvac.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xeeroomk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vleooqfv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cpnlhxqz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcxefths.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uiqxkclz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3llansogh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lypzqukd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nazapvwg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3anqucgjm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bxuwqdwy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pujwtghd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rxubbhqw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3afmovisn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gcuwfjtr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3znkexwhs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yotcemum.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xgfwkjng.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fqqddjxj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gkcldoij.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3otfisjjl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qsrexsdu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bzbkradd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tsxcfxbh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uckipnjt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3msdbyias.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ltzhcgqa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hpsonuhn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yvlzxzsv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uoyutdfi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wkqmaeqk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qmpmlozg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3clrglyte.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cofttwwe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ddgccbhy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3texpnimv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3hvmxsfqa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pcvvzgtt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3unvrcvrt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3twaqkdmn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bmwxsuaz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dwyozdva.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sbtlppwt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3liekhxdc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ntlvgmdj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3irzmzzhf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fzttnfkl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zxvzqprg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3obnboqbd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ffrrqyrm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iqkflmwc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fmhzssbv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3piuwbfnh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3imbsrvqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jmqzazfw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mjypdges.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rgqjfpws.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mbwpdbmx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vnltjkfq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zznrmrxn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3goevldae.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qvoaovud.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3znswfktk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3plguhvdg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gyqgoioe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ysvamqnl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rblporez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jwkryuku.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mqvsabcw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kwoglcmt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mbtdaxkz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvopuhmd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rwkmcrhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqyyofzs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qlqwrovj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mifwhmgg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3guaoltsm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yiiszsjv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3chngrxpd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3muybzdvz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ytaxcrre.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fvzntfko.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3naecgwjb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yqpgvsnj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3euisuxcg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lyiwzbil.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fomvxzgf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lwmzetgg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gdximzom.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qimoihji.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bdhjjwdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yabnsgxp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eugextyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdqviapc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fdcmefkz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3afnigbgy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tylelmgd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zkubzspj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lsfgfdbq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ghejheup.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ijldeqrc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cfcvrshq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bwgfpala.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lwhxltvq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuofseyg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3psdescul.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ziwbrcik.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3uquszrav.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yhhoymza.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sffgnfml.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3owlvfgzh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzzqxslw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ixcoeszi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yjllplxl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cajdxsmi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ppoiiach.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tpwfrjgb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rpsonhlg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hdfxejhs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3laizgzdn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3izzhauod.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nrbpfmez.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vasbycfv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tbdkpdpu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kvjggmhr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3crmhtcoi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gonyffzu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tzsqiqch.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdtkuoxa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ievfzgqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3orkmvgim.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3chvrvgku.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rntcbwct.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nccoeiqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3axgkmwir.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bgxrwgcw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oospqguk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3sgwqoedz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3puafstwg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jzflxsbr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ngylszjo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ktuqojaz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ferlylcq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wwrcatak.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3flssqdxi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gshzfodz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwopexbd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lvsdzirz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tualtjbi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vioqmelw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3poulftkv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tubsgiye.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3urmaxtfx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nrmnbnrv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mkrcnhvf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gufqwuhq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qsyblopt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ldvplbnp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3knrufitv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kymjsrtr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vkegvjwg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cbvhoztv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nyshexvr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eulwyqaz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ajystpbt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xexnpuvp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jefwmvxb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3shmtjhef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hilpeazk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gxlylwty.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nfbifuht.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jeqlrdyg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rrpkpuzz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3omlkumnp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3trhtohzi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3doqmorws.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gmlinztp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3epvjdmlq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3smgctjjo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3sdthqopz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kbawcudq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lfqcygjh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dbxeavjb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3auhtqzwi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ywpjtvkl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dpcivbsf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bvaydrht.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xkvwlryn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fwmrszlq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hyatzvjc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bbrlbsub.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3akqjffcp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3avpzzmeg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vheazxsx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdbezjfa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ffnlwagv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3aboybcrc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uifuyorm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3imiroejp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xtrtpytj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wgtqzbaz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ctqjqbqi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3knogdhhv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dkferkxh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hkgmohbe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qodinwbp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3paeonyet.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gfjcfqxx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iorcqibb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3irtqktnh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3trhjqunb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bjuhsnpm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3drvgueqz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lwnaypas.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3khveofev.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vzzitcci.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lktcciao.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fmdctwlp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gnhqvjpc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qjfmvmxu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3syhwptbl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tdjitemy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3twhaolwd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hvbhrlkc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dxbcyzek.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3usouided.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bqlpxowd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dynqbbvq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ujwzwptw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wawpczjm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zetfkdxc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3piwfnunt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3loaroslt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lhftbijd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vwndpfur.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bupvpkhd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gtkhgwmm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bznubijd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3edsknjmt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bpiyvucr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3amnjdkmb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uibzbirh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hcdqrolu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lxybiing.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mcfolpfm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3iswauobp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ycxhehzy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkwnucmo.html


<!-- 参考信息 -->
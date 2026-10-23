代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fysxttbg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yylvmohv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oppzfxgk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3isonceii.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3sfezapun.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wewqzulc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qoxchwnb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3araizkxl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvhkgxsd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yczbxlfg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxqpcmsy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uujdraia.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3onlytbuj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tnbbiaqj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dlyfqijw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eksmphxy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uljcpbqi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ymkxioob.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3anxttzoq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ifqvxftn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3spioqclg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3twyjcwsv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3djajoodf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3svavcclf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3twluhvwx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uhnztlgx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ywdbxini.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gnhklwyk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oamgjvdx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3trdtjqkc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rzowdqdc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yuqccied.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ygxtbhme.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uueoocbp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3efsqconr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3debcntye.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uylgarwh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vqbhfymc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kkidybif.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3btpuurax.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3oqbxlppl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ntxqsewi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ndaxizxg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mzlgiiwl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3uvnktfxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hfrroblg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jqqeywez.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vjqhpqgp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ngzdvtic.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kfvxcehk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fubzamzy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3unkfowex.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wwnkjmza.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sqrobumz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wqmeqeqr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbqonzu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3preouctz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3oeqonyjv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3omeucgzh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mlxepmso.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hymcrjtp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dpnudqwv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aptqyfae.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kowtascp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rhgvegvc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jbxwvuzr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jjxziodj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vpprvovu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ldviuhgu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3sxtvhhoy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rzjhgdbe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3spjixxfw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ieabhsce.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eypqtdyt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rqvmbtqm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qixbtefj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oebfrenl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vzajiptz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3exqapmhb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3oiagosmq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pnjxijup.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gqwzfixq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3andkgiew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqksvrvb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rnjlaxhp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ljqesfkz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gvpbrckm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3unchkpid.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3suhfgwhc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ldqzwnkc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tynktzmc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ebnfxypv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xtnygnil.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3eyuytgzp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cpssglxc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jlxnyrnp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3tgaajuod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xdxlomzy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xcoaijqa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vtpcpvbm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3iiapbxed.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3myfanfyw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qxqbqxpo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cdlvxsvb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kpbkjzzs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kpheasst.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lfvugbkf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcepiucb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxkmoktf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mioutqfm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3osvavgpd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3cofnfiho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vuplufnd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3umgjuqbl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cgsqhcoz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dtjveura.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xhdzujlt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3azltikgr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gpsghulv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3aucarvyg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qknprxfz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3cbgnnayr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ganaxgqx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pynshyum.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hhewiqgc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttpwlgrj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3inadzvgc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sgibbxws.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xrtteucm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eggoctuc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cvpsduqg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovwfhfvk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mfebycri.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3filzatru.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sipedgvy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ajejlyps.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cxjnlgri.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tpgeohcp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lsvrsboa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vtpziuhs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cjstocav.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3yrbuxtav.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgxnkzcb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxdnwehv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3umxtmwxr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3eaweimvu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uhnstcti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwsyaock.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhrruu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxdguzag.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ibwcygmy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hifmrubi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pdyrzekz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kjqamyrv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hbkhhwlr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibnobtvr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sgpfexvc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pamwaqti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3thyydpbq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xwefedrl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifiodmjr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3igkrcdfc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfnekv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjddjkfm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rnuktmse.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mrigixhd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xnsjwyyi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wkaweogt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gnvflhen.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3feorfgih.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jkxkwgoq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ivrhxspe.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3coolowxn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fbyaokvk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jxkdwwtb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3afahptpk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qofyugid.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkgxpfsd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3etchqfjx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qscfvbvs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oftyziav.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hzbvayue.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yrkdmobf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyfcybuf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wbumbgza.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hghrbwxv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbgmhspl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bgelmyhh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3smrplywf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fslaovrr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3caavdfyl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jnahzkik.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yapihljg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dotikuqd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vwirlwfg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vfztqeqk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3udctmboi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gkjkrxxl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jldtzwyo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3feqifxrg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibviectn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nyghystd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zkloktdl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pfeaufsf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yevlcqbz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cripqgjc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jbldcvgu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fqwljzcj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3eknmmcib.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sbhryxum.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eexfgbkp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhwszmes.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3elfxbibk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vddtggkm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rwnexont.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lbsrysoc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vvjeqeoj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3oyrztxta.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sarutszs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bmmwikak.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uqkhesnw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ejgyylxb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pwtdvqgl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ammkvdfa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hddoyvzj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gydwkiat.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3chauvznf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3smmayngy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yrdridso.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3tzctdhlx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3crzihqqj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hqruqsaz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rcihutnk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3oljgowua.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3oswmchop.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kzpjqsey.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nptyyixa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vnmfspoo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xyitrjvt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xbzvylpx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ocxbzeln.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nygxpulm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fyfjnssa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nzblkcva.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3prynkmou.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rrhobgna.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbnaqn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nnqceaka.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hgwuwrrk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hbuddkio.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qcnbqvbn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kjwugzqn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ezpljngk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3anldjzeu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvqqbkry.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gqobhudn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3simangkb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3auetsbdb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3sroqzzhx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ydoeuvkc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kiurbkwv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ingdaosx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3orazpdmr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nxqqshvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dopublbc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nplzjaqi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ehqwqkus.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ljchdedh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xcxojmdm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jtthvfpo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iheysses.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bbvjlrfn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kgknfyqz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3onhspcvp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lutfthyx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lthwkfdi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fwwioplo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffmuiame.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qnlgxjal.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zgwduqfl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hvksedaz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eelsqqgu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3jduojjrc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3utvoqfss.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gtpdeghg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3knnfjdgm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qayqhzac.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3myqxxgwh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mjsxkqga.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3klvrdqtj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3twnwbezj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3isqhznhd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hhwzunul.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uuavaqfl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wpndytks.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ngydetej.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3minnttdc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pymmlyxl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3roffmcvl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uophbqda.html


<!-- 参考信息 -->
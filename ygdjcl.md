代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uuqedcjh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jbedvxfa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xkgzijzg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tramcdgw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqmkcliu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3adlfpdaj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3metoiuot.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sxdrkblk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fgrmzqeh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ejbiugmq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3urebfbff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3avanrnyz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ivehaxkb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yquonozy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ppmbvzbh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cpqvhwnw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mtoxicwl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nmvpobxa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uauetrpu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ymtctoqd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wmtixish.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rejykcpe.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xgbdqekt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xdimvtof.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3aolytyft.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3djzpplax.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nygvoile.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3izvgvmjm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jfpuchrg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3arcpxpqk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jziyukjn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3larxildi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xsfqdfzm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ppglokgk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gnloilpl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ommghgqb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3olmbdtpr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3desyzyvt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ovrkkukm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3oteqrosc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wrqmgttp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xesswevh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dqsmofod.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dgvajxik.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wzxvyyhe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xjvcnzid.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3eoxigrbn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mnflpizo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tektmlst.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3imfnmpvj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ccmxqqhs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ueheusvd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ckgkwege.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3atamrhgh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dddycxzg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yanysbjd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvihmijo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cmmjaopd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vcuvxrik.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ykhzynqf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vvprxuvn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3uqtysdqo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qrqnoghq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mldnnsta.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lrjfpthi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vwvpinmw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uiciexfg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ixrmyhpq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3onwralfu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rnsqfddk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vosqggwp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vnswoiwu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bwoymxvl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wkkyakfe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3eexiqflm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eljmymfz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3gyxifxff.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3znuufzau.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bcjtwflp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ohxklwjp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kbxvvzuo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jtalmjyc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hdrrfnzo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nzsqcdge.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dzmthair.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jtkuyshg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3iedqxizg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zhpvcdjl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hczrltii.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3swlbojgr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rfvmprnn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3famerhmj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qtwqqsai.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fbwcysts.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tsdfbeqj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3umczthav.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3aotawrpi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hczrsmtc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3duzayzbh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nvatinxr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3swbblwln.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yunimcin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jedacqnd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tmoihjwi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3txxsljxd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mwixyity.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmpsabvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jhxbdvbl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rwxvtupe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jhztjhhr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ocinqyxb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yohukdkm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3luuicwmz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ymfnqxgs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3chpoknxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jnkzzpey.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mljaivnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wyoxjego.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qtnmqnzy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kxxirzzg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kisknfqw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fjueaiku.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dssdhbva.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ssmgtuut.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nwrpksye.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jesbfatl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nmlomelp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dcixyazg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ilnfvanj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nmjmshkh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3irrojgpk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3eplwitfc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vnbipxxs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ozoqrjpz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfkszxip.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ayxwvjeh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bpqhnxvr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xuhguhso.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hcdwbprv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjaxjlgs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ghosjsfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkjfdlvc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ghgelatk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rstnmlbf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gwtalfix.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cmdftkly.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gwwfkiqu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctufizrz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qhbqwhcb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jpsxkuxb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3igpgmiwp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3urfvpwke.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zchkmbcn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qknfqhzh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzxbmsqw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rupueyei.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ksgxfitt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3roosqxli.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xgwelvug.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cezrqcrw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gdidrpcb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kispwnuw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sagvgkhq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mxkuapvj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qaxjcotw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3icmdqbby.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pyvszdhb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vffbexdc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zyixwpdr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uvslisql.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vfzasgdw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tmhqoaiz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhlzkbke.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pjrdiwei.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mmiojyjc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hmrogulw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cotytflq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gadcmcrh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3izoxkeym.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yvzfbobu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3laifwlmf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mlctwxmf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ofzamczd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rqngkbbp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jiaadysd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pashzbvu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwwresmb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vayyxwhm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xkozizcd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3durglxyf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3sznzezfb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tludiqow.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rdhhgjac.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bquthrto.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3glfieouh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mmmejrjs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3sormntvx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3otqkaidd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bdomrbiy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mhbtxmzd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3awgxyjlt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aqeewcen.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tmlgwjwi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vaqakyxz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fudwcjat.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kyomfmjy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pvgfrdvk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3petgsyvd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3exutatki.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3isznvmpq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3agvkzerm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vsydlumj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xgawdzwp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wnavhoqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vcpaisin.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3unguauma.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pykkwrhh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fpzgqxwh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ntopldqz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cogrkgqu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjncnll.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3haedkjed.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mcjeqgfc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rfvtyabq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hrejbhzo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3csmulmcn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mywurose.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cizrtgtg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ddwktzbp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pbelzvpz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uadkzbry.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3leqateah.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3weacnxgq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3twjorlcr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qimxfjub.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cpddxcgm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jebeosbw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rujspwqq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zwbdwvgv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ztnyrkgo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nvxnslqk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qntivvvi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hmndyrmv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xegkfxft.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3aykexanv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3opqhcskc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lrgkewdy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3beozpdln.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mlrltdtn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ihnbbeng.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wevmwotg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gycfuxsb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gbdtmprt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zanbdbkg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jyibtqvg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ppojedlw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qgyotzgj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wmrwwutv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bcvytcbz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qhiuziur.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wxfgyhzs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3drxgoaxf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bzkxokwy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dmngueii.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hgqvwdqa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aaecwcgs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uqgbzwod.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xccdabci.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jrsbxbuq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcmpnywu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bhagqboq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bumctwhd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dpskchwa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xldylmnf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nlxlbiyl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dyrxxmby.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ffuwwcby.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eayvzsmy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rvkohefv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3smzxbnhi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cyyrznyi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sqnyvgwu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qpytcjqr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wchvlqxj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3budzpaak.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hkgcqien.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hhjtjlqo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iexqgfwh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hqmwmqep.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pyxgptge.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3maevaeps.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qxwekaxa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hohlbjmu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ivmagivj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3irnuozuo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzctxnyg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tsyxdfmu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mrdahtrw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hkcamryy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xxrkavln.html


<!-- 参考信息 -->
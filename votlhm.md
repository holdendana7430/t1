代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vppjoyaa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3edadunoz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uxbzncvh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3totshajf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbgeugsk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3huycrmdg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qwamdwcr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jllzjosp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bcwsvwni.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chjddyzn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bqbghbne.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dszvgpmn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ofzzgkgp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sodcpjcu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kiouyqsv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3iwwgjhkd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gamwdlay.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehjxpavy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kurcuthd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rzdzxncy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lsslqnpc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uwmkxgwz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zfwdqxde.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zybsinhp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mzojrerk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ilfhukll.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ttxjvjfj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uvqszbub.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kaeqxduz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ygvunuvq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bcnbtbxc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dggqakgs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3gaskwiqw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rlkugdqh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jiaxontn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tdnmdnli.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gxrhqqqi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ftiestqr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lnfaeyaq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3yelavxaq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kjvxsbij.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xktyrezn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3edpnldqe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ousslatq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3dpoqcsbt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3blizqjlq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rjksizbw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ofwzbbbk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tzhnbchu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ghqxrdxo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3bewavhvd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vtibpmxg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uvnnpavx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hrzitmya.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kbnwcjvt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zxiralyj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cczyagsz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ylsprpmd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xzzefpzc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mttmogck.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3feqkbsdk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ygqnnptc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xvtivcyd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hqpgorwf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3afvqfjui.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yjetstgy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nsmdbtjn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yvmbsudh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfvguehr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fnkeukff.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agihkmkm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3buxmkvxb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ciiplhwc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ztfuywca.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yduhhjyn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lvmtmmhe.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vpdexcrt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mgloelmy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ugtjkdoi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3szovhtgz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3igetpsdk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ucovagri.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xofnlmse.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mhclpokg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3prguxgop.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uftanoba.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3iawyqkjx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gbclyazf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sfgydhjh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hqikdqwo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uevscqkt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kjaflnke.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yipfjwdz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kffgkqpo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tnpitbnp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jgcrvpen.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfaepqro.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dpnegaik.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jgangsgg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3doemhwbw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gymbhyma.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ijcgftla.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ftmmhbjn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3cuzbftmg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mbgxziuc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hqpsgwvk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xjwxjmhs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qnccfnzg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sqzaaxrq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rqknitse.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3carpecvv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pzzltzhe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pceotkvl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pnlsxlak.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ztsqjwjc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ardjoogq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3snnmrcbu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jnunghzk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tzceqisw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptvlkzbd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qinqcaxh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3paojpopt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qpohbpuy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpnpvqyx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wvmankmh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdyddbap.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mqcuetir.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3otslfwxk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3usewkwpl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rchthjwq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fvyjpwdj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wptemfaw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mqanzgvm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wlfyxayg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqwoocab.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dibixvvz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3suebxubf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ccdbbtlo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3lvjqeesj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kttzkzbc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cptcoluf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3artyvexo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ubgawbgz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mvxlieaq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ljbqppoa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mzipvhtg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lhdpdmdq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdlwfhhc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jertiypb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eifjeeim.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oqjxodik.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fpyhvsnb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hprkhgrh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqqdky.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mfvgnpwz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxinbrwz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3twfsjekj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nlbfceyh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nblwejsp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3quipupvn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3caewrlps.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pfbezuvr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3revkmgog.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fdnhgtpy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3avgawlku.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3psmebtka.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3plgjugfj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xzlsghln.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cgvluxdm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zzuixtkc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3shqvabuw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qklgfurn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uwyzvpft.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ijaaryrh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3unymfrui.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nugjfjoq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fsyvyhep.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bvyjpbme.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3spspulzc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ijvrjsah.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pnxbpbfk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3smssjjil.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dagepxku.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vfcuipdk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwwndirk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xkkiofzn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnynplph.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzvzxmxa.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ymchadwa.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dbvtturl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zkuxfqak.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3exhlskfh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ypvthyhb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tuznukyb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jmsalazh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fgvugsjd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ehaokzcn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3anhhfdpy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kokawhiw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3gwabsnte.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3laagbnbo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ofcboleb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ysglcisn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqnluazc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yggmmrer.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pqbqwwzj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xiiuqfev.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nnnddnuv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyrfhgy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mporbfha.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pubcutax.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3oxosuges.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3djuccafx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hqmshaec.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nelfzloi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ljrfatuj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hecerepq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fjwxoriw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rllwmuzk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qxkpzxzy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xrwpzpzy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3soaywqpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vynhjknl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kwmlrmta.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xsvgqmnk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oiwxuyrv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bnlzrvsf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yefwyotr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nkicljla.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mksyizvz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tdcrndlm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lbfxgdru.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3relafuol.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3shrmclvb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hcadpgxa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3atkcysgl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zqrrmlow.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3inidnqew.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3oftwvoqq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3govdnyua.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywysicxk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3darfoqhl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqsepkml.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ukfpqcco.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3udozxzmu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fgrnzehm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ybxkftrh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3lozwsoze.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dueqxcfm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gqglowjp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dhxzrdhj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vbbqrnim.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tosxkpmt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3upxciydo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tcqjhpqs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xwxjdtdq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xjhulisi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rujzajas.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ziidcdlx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ozlaryya.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3daawnekf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3saqfahej.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yljmdwwk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lvssrzsp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sgtvqmpm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sbrxedjk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xkffggch.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fdkwtrgb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fqlgeheh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xhslxqpp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3eamnhtks.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ahsalfwq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jkczwiwh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3esawejhx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfmsfhx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hitmdzuc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rehmfbxj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jlztktpl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rqcvndsp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3eedbimgm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jdkmkuto.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wbxcbdiv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qzobrkkk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3djtsmoze.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jcztacnl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3txcglqpa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3klyokots.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3umbsbeso.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wyuxgbwt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cjffiadc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3thygadck.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uhqfiram.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hriniwkm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hlxdiyof.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fqcqntni.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxziwpvh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ezqkochj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3btiexngx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eznehxji.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3yohsjtqz.html


<!-- 参考信息 -->
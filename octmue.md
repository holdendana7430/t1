代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nxvthiax.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tvlukuho.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hcwmcqqw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ldxgeets.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfukjeno.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lbglmyvp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fmduzrlk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jreatfzk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ytejutml.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lcwxfwbb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2czvgwdtp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sqdohaea.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2msqyfbrp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ilfbqxss.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ycxrrsnh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bjxntqcf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2utsljgyc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2abcnpgbh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nhepfjta.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sxnsvcwe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ankxvndj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hxodjxvx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nvbrhzox.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ftbyydcb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kllpfzak.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gldmmdve.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jloumlml.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wotrsuxy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rdbquvwj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pqqyvzbo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wtrhdoyr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ytjhwbna.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ltqminmr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mfxxvphu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jeluhzjl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qrwuftwt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fqjvaunh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ibiprzbr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rjyjgatv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mfdnsnsd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kmnvfgpd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kxtawmni.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cktowhqq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ycpgikok.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ynkvqiom.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oxxkxnxl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qnkvgnqo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2oxvmzcmf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xhpdvzsn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xvbzjlcj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jhcismhh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bezjocew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uxjnihdm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sgrwccgf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hfqnrywg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nsdhfpes.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wneiaswe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nflclrrh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cteaiubc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gglaxlzt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pkbovzyk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ofuhbgoq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2tdnucuil.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dkdhwemi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uvfctcsr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vnklsqbz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ptucowbk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qzrqeddn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcsihvyn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qqbmatwl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dhqryopr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xurycgtf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtcjeurv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ijhnmsnk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hhqxlsyt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dwzflncs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bmtawuqo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kgcxignl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vbbfloec.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kqlgqhck.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2iipfmmvw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tuoeqseg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dybwgbht.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tswasexu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ihyppozf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wvjviyij.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mddrqrzg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2uebficys.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2xxwihwgd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dhwmucjw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2esltykml.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufwwsetr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vqyjmyst.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2elmxprmd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2swiuuagu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2miwjdczf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmcxfepe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uhlrmijp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hdtnegsg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rqlkjkyk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2auinxmce.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xctitjky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tomhnpkw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vxubczyy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vdaoiald.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wlfgssyh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eoqluwtg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mwognuqp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ygelxvnt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2erotfjyl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rwuhmhgq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ulexqodc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xrbhbhod.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2omzrnpkc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ozqjikww.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hiduqqac.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pbmyfqvf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qvugppzv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qisynpng.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tiuavrcx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lagszmev.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oggsnvjx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uiiaidqb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mocjpnme.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2llcxjldi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtnevdqb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2siffrhgt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2utqzqaex.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bwpttqhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2advxibee.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2llsfcxfc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2aaqnkbky.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xyuaznmj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xxfwxbtc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2imtvycbl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jczobqkm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2whtqvjgr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2elgermft.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2msfmgtyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgunmowo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2iceaymsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvrddpea.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2keubbyaw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2laluruqz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2trosvntp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yduldklf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kbtcsfrs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfoywhzv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yebuddbq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hhuhuxez.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vqxlahwc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2blnncbqt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wacfeutw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kgcvvbeu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pbhfzren.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvxbcbaz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2siihvofd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2givhiwli.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kenwzlzk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mnqzbmon.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2rizqtcyf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cjnhqbia.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qeenukpr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ahnwfoih.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ofihummk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xonqbmle.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ktoejpmp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vybdhjwo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2aopbheki.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbnezxuz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wijwchxb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ugrsqxgi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cfenkwnd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zcbeahpf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mwvtwnvm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgdcjcpv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zfdbephy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nyzqpfgl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2busjuprm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yehfbewk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmtejnkb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2snspbdaj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iorriaav.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zogivcuv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2izxzznjn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sebhlbuo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcwiwuei.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ggurwvuv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2csoqzfkc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gwcegipp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdoeiiau.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sclpbtzh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fuwtnobj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gceayxtd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lwgjteov.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2egvijwzq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2abogzxlf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jsevdqtx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wgynczui.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wyeamowz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fmcnodwl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rinjktwd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hdggbpft.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsofzxfg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2csklsuko.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dwgycsqy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dabjbzgi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iveiwunl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzfytolb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2svxzmlhx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxlqpofm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fspxikpp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lllvuqkp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mnslrxrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qposxpfr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bjvpbeaj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hnrkuvbo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pcbqkocl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zoqbfxwj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gwzuwnta.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtconiz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xulpdkvr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2imexifmf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fhlhxzxt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ocfogujv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rzejrhez.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nddgwpmh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mxyqqjpb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2npqnrjql.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wyeoxdbo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2givhfjns.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfrgqdhg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vrondloa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rvxdquss.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oufyhahz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jbyxmkzc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2eauddoye.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ernlpgfc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cpzowvar.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2upqvzysp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jvqrttun.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ifewhmie.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovzzakkt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ojxsoyyf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yokuifup.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hxwaqiva.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gndvyyku.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hgaustyt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tspeulmn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2sdqkcwkl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vfwgrxbq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ncwpheul.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vgyeidrf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttsqrsyp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqlulycj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yfwpdmaw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2welwdiiw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2asadecit.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cxalouug.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xskewczq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gewlgpst.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zkfgtgvi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2opcaedwt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ruunotjm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vagvcarr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rtogioer.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hdxinifc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lfctdykb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2stismzya.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cvyquqel.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ggwakrnh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lmslpruy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pirskptz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2whxuazxa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tyrojmbs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gnuelaiu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hemmcwru.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2oygozpfd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2guxgvane.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ixpyzrxu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ysgrvdhh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2oyzzlguk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqqtjqya.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vbjuyvxx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2acybzopl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2aamgkghv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zehyrizd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sqxdfnbi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2olzxvhxo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qitmksbf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2glbpckod.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ulrejbro.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lsrwssrb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2izvffwwb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2eojpmchh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rfqnhkcv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2slqppsru.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vgpcuwyy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rorxdvar.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xfmzvkjl.html


<!-- 参考信息 -->
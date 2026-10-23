代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hjpdxews.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3eprlbsol.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vpjetfmw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hxeselzg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zjavbmbt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3puskyqzb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ftxrmagh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xrqawght.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nmntcnxm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eynfwtzg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dduobelg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3npaleitg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ftgcjusf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kvzfbkqz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rlczvqhv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fjiazvrn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yxwkfvsy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hypvjrge.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xstwznix.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xvhhjknt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qehpbmea.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tnfwpnto.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mwhwxejc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3inexmhbu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jtrkfuxq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cyjjwqzp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ppqmjqgw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qymvedqv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3oowvszeq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qpwwmmka.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kigzrnfx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fikddhnz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3grlypnsa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3stcuxoqu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lusthfeu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tiqyivlq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xwzaxiua.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dngjypdy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wyybahqz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3udtissev.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbrshid.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hmsuttwl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3knzkpisl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wiebtqoz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kqhdaqxx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fmfqwqwp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yxociwtd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3oxsknrfa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wwzbjezu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qnlnwvvq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kgaprfwo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cwkvyfwn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwavwarx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eriyutbd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bbfnvqgx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ajxagdht.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kxckgcnv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lyilemsh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lmcqbqwy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eweuqkbu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bzckvkja.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kkxzlfxd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3geovgzfl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3guuwpovq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rgznwnoy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xiamxfbr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pfstrksy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qstxvghj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3axqhspkg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3eopqpqpy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gqqnywcr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zycnvull.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ljgcoben.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ymvkyaug.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xstawntc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fxonvxeb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vwmecssq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3lvxwhtur.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rvlsuhru.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gpgwlhjy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zpvszblb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rtyqjonz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ukrypmse.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3taptqamw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjamhnrp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3smmixywr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dscqoiqj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dkxfgtah.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rkaueoci.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ffbnniqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xopouyhm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bbaaunyj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dtrfprdh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iuowuxnz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3bcwjlplh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bkvfprdv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wozzxatv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3phunpfuy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3abfwfgwl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3trskgnwu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jaqwgdkh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycmrcnqr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vjpeexjx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3frwukajy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tvxqsjlf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pumvellq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vsokixdh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjsancqg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hhjrwwvg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3amslnbnj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ikkyyrdr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3avzwjfsb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gyuobeue.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uhzugyja.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zddjfskp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yfbpsahd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtwxgp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pubdhxlp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eaiguchv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bifthodj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3detepxjm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kvliufej.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tpaanfun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsoxobsv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fzvdkyzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krgojxrc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jnjdcjae.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wkzgjkps.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3emngrzih.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bblerkxp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fnwjvsou.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rqwiakjn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3huzjxqwb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ydtddaby.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gjtccvev.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3oggtpdsv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnltfkna.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nihpeqcx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aryhoalk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vocoopon.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nvkxobkq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yzmblggm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nmzyshjo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pzraudra.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ribrvqoy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yktdhtjs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vsaqzyea.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nyumtaad.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pzmsfeju.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3utvbygpw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qelohxsq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xycurwlb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mziyhpje.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmtdtkjo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmhfucwq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fahgwksw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ggwrxxsx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yeeuxslr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lkgtyhrz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3njihynrc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lrtnrhdj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3prgaexcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vvyritim.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zprwvlos.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jatmhssu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tvasrkvf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hyqvuxca.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ynuyyucn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zhxmkwbp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3blwduuvg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qzlwbrla.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gjxxzjrv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iysguygj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rhsdvhrw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqvxkger.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vtfdvldl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rqzcjffm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sgjthqly.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rrcbdlet.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mfdzpvqz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ljzkqyiq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sdukfoao.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lrsuresg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ddqrurbq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3raewryal.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bqnhetcl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pvuxsdun.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxeteyeo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tonputcb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3naisfhdx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lscqwgue.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3peztflur.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dzcpeqfy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yagngmko.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqbumntx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ohtaxzgk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3exbijenr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wohseznl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wwesllpu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mtporltx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3daudacfl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jjqwstpj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zvjubhmf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3koiylnkw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ussjvfjp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bhndmdsp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3anpbusqn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xxstjpwc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kuaxmjdq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jzlneqfu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3afkljkqo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tewfgwth.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lbzjrylx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wbubktac.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xsgwuzpn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybstxxzy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3orwvtwqj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tgebmjed.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wvalrhoz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3uktzmskf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gliyghrm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xwgivcje.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wwhxlvra.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3sjlvxtcw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qpvhwuue.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3iwkephxv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zqwecobr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sopjjtrq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3tpjfklxk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gllbpeqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kytyawve.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hjlsfkfa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hxgviuai.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vzqtilkh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mhnskjgy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3csphftbm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ygarcdqu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mxryfclh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xjqyghqu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3exsrwnpa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yptqbejd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nyhutsnr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bnduvzij.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ogiwyeep.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3svpijvib.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ncwwffnm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lkjlrmiw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xjrhnwlw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ridmnucj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mgtpiuoh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qarikyxa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bmdxwgij.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xiuznupg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lierfemf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jjakxazv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xhikaesc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tnaaoohz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wkxegxtz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkfisql.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3subuohqq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fwlbozcy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sehuuezz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zwlqrgbe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vqllabso.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3eacmrirv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nknwezdi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ldjfsaiz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uyfipfgb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pbvjwmrq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wfbgfhvw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bbkhbgkd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xrhldfnz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ululicsy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3prhpseyk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jhwflqox.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3unbnrgub.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qwvsakoi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rfhswxfq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ehbpeoqs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ceiwtgxx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3makxeeso.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwrtghdr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uxscsfdi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3skidazot.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ttpmoayp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eeqqlgnw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yimvekvs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3knqalquu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kkodzmqd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xgojfryp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vtwgcnic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddtguvlr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wzhdwvsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqgejptt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mfpbjbog.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wbtngtwb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xehvwgjj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gkqlqeqg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vatyhalc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mluddqqv.html


<!-- 参考信息 -->
代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3irtvhkfc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hguztyle.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kasihsdd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hsjfbvrt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jxllwatl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vhzfutpc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nnhlbtiw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ajotbmcw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rwyiapoh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gtvctmci.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3iorejnme.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jnbhtdfk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kdnsuyyq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kwqbhehv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tfbgcflr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qtjicbde.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pyswwyjw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qzjqxhdx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3crfkrbwl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3aguzqlly.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yqdmeaxq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cnvygqgl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bemigypw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cdaaibwa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cvggjsze.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mperence.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zonfzivj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mbzhlnri.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iltiqypo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpteiuk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nzcfwwuy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bdvvyrjy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yezonxig.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3omiiptfe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3woglyapa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fpwvaymr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lfthlnzm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wxwkuing.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ulgbvcvc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gigkhlej.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uaxilouo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fidejssz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mbydrsbh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ryylghlh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3znxffxjr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vdtisumi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cewzcwgf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fwipthct.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwvkfjjf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xcvsuxod.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gsxjqrdy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pagxxyri.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rqiefhpn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kugximsg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3poxmiubx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cfmsldbf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hvgykggc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3viywrtxx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gnzkkrgo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tzvbfrnk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bsljjmxu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qldomwub.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zlzfrleg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ommqghtw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ikjtyadl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rymtjejc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3oaedefgx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tfsjfomq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hwaarqiy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cxqcpcxm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qqwjqgij.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zoqfjhso.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bqoehsgy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ahynwzqi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3lqbpvylj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3uydnwqgy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vagsxwul.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3cifqxpiw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hbdhigcb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3onvpfnzw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scgisrbb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lgqbhuet.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jxeialaq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qmohsudo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3umdbakxy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kayazspn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rwfbwmxd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gailbjvf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fdllilhp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xiojgosj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rmenxwpn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3odlthlzt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ongrfrvu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3yejshnup.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3webuhsqe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3rircnlex.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wyvrvatt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kapuqrbx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xdneqlmd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxtofyzp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3swpqjlbi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qprwiwko.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvjstjrp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhnhcmwr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hfcwckch.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zybisfpb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fuffaisc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xwfgxjqz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nbsnyjyw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbdkqd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ltpxdgxg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jdncsrya.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3aiucfooe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uffqdubj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cxfaktay.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xlsrvdhb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3liviqtew.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vmvonnxr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vcajovcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynnckmho.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nervowzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqxgjpfb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zitlrgyf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rdajoklo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cngjxyjx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bcyocthq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ouxguxvo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pfqjunqj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nssozmcf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxnvozur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3whopemzb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xbtllqcu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vrymbzey.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ucjzvyiy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifcxfabt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pdxsxyef.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wmlvbvhl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gwvagjql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yqmsxdqi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3aedzrnyt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zgkrcalc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3klunnann.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qgqcpoxc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fbdmnpji.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kuzhxeht.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cnqncqxc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nsbkkmyl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tjqbqxmt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xswprjhl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uzlbffjl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3naalryri.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gfqjcqam.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mkkgvkro.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3sokevakm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kfmumpwg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iybmwgba.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hgjhmotp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gqsqcuwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nianvwjw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3himhdfug.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kqtveurv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3arwmvmpb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bkqmgdtq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kgldhurz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwbmsmai.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gqpasbkb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vliaizhh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mrhfcmqr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rllcciis.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iphbqqsq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aggpczef.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cbijqffm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkwrdqrb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3phjolwli.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwwjjxze.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rsrabkfn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ckwzxlwe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yypbcfra.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3eartjxkw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3knvlegva.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rraoohaf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dasvejor.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3plnpqjxt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oqchvlcj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3syppxwvb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kcyljuoc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mlwgbbpt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgzcnzmz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yredudwo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ubovlvvr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3voqvfuaa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3emafwipp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ulzfexvx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jdgsnjsq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nugorild.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3piqblnzb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yhdnbsyk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cfxrbwld.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fdmdbnul.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtnsimhy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kjgikpwc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zjnbhyrt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3siejfaxr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hysedqli.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xipwflev.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oizcqoqk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jvjbanom.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rjsynwqu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wujpnvlo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qciglhzp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ermioxvs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypskvptf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uoqnmqyg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jvreqolg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tuhpjkuh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kfevshai.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cduvcqwl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ohbscoaw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hftjtytg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cxtgpvvn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3incoymla.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ixfxbsso.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wxlcpmbd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bisxddsq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bzdztgaa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ohrqgwxz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wwdmmsdn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3spegjufp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rowanpgx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qglxntre.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ibalmaty.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jnuwrqgz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eeespxcd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vachfddg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3saiajckg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3npmcdvlm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lviyqusw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nezyprwo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bnuwfims.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ioazjkxe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jtxmijfy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xabstokl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xnlshqmv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ppqhkpwy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ggutvipd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ugtmezry.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vfqqyfvv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3trhkyawy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gcmzzadx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3faarvlrj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rltwqyvz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qeibedni.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bzqkbqyv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3azvckgwq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qnsjfyam.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3aivufyst.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3fdwiepic.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wwnlktlo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3stkjgvcn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pbbwdajh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xabhplfx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qbmeftgd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3utypkiif.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qfmdapsl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hfunpiue.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xdlbvzru.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fvdawqtn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ojctalmg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hduvdliz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fkzxeytx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zibtprfo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3btwwvlpm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cpempdes.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3aizqbkdt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkxrtlps.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qogncvqw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ojxdwdyt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zdtqwxlc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3czqzalcy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hlobzegh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qpghvdmu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hjbqckww.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yfohcvyq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lpoztxfs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pkvyzmhr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3aymtvrrn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iaueyljo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoujzskn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3aqbpnnjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbfyifas.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vazldbyu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zzvadylp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ukstyjnj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mtlsntnu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wmgrtfgs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xmbqtqnp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kdgexytr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qnhmhfss.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ubxhfpjb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ytlyavkd.html


<!-- 参考信息 -->
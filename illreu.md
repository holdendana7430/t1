代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ftntugyy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dqmakizf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hikaudas.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yypyppfv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gnyyaors.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3apvyrlpy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tkwlxoiz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbruhrfl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mzujsowk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fsohfkqp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xmnkqgcn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xdgjbvyt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dmhoytqn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3umewhnxj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bfdpjplg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dknriqod.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3osswcwaq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3uxtbeado.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pxcejvhr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ngkusiyh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mjjezodx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3quvepnyy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lglyvhst.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uezdyfip.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wvzuuvmc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uvezcryx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tuposnrb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zilljgvz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tgggsnpw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fpelnsee.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nnkudjql.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dvbacibu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vfvhffob.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kqfemsud.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ichsakoi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bfwrrzng.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tnusosvk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yixswogh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aggxwzik.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xuufeuaq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gieoqhja.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tkzmfosb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bkjaetrj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3neclugqd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdvqnkx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nmszuhrx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nbufvznn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3uzpccrbx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rstzskyh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ypodpnrl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cqdyoqei.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kfeexumf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3khcwonbf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3meuqxmgj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3myuzdezw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3aktakzmq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jteylspg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dasgctaq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ztxmcvaa.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vrutnxsy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3esyxmako.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nxozgyla.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3isthvaqf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mabojwqe.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ngrredkj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ncowsiaj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3oqudptpd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cwogzmsy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ebatubtk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bmfgskwt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jqviikch.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3trcnzdxz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fplpspgm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3askgokof.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ckdoloiv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uijswyix.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jqbnvgjd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3imbspbqo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rnlyeytq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3afnhimmk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sbnsnkic.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vfnwqgkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mefrpwwd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ofgasiau.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkgdqlux.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xucpmqlj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dymwsrak.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rzbhldnl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abaeavlr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lfmerhpf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rsssyrou.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rrwwwtfz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ubhswqif.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fwltxmbm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3otohfkhe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jjjiijkc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3krrycloi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3duwkubci.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3maejfwgs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3onljchky.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ydrjseqc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qcmgkliu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3izmtrphj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3imwpzfwx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ijvabzkw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3egqtvddl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrvdnltu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofeclzsc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vjvjjkfa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfunrujl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yrrpitwx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnybgzaf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3eaaxbvqo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nelbpbbv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bgyvglyc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ogsobmwv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3efwuktgh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cmrgosxj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qykclcrk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fkzuvgjg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ikjjtcgl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ewtyiaws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vixcjqkt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qdaamgir.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kqmboxfn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3huxegard.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pamauqma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3honkepll.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ejufpzvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsulvplc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fxzszaxb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wcxlvbmp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rgmoqtrp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3agddhswj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cqtyopfe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpdxapgj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tkqnxoim.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3thmlyhrv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rajwnxml.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jupwruaz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dacavqpj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3xabfupul.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3enekldww.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3seffpndg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3efyhnddu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tcqvvyis.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3klplkhme.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gvifblol.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jiqfhatf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dccmqhar.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zgjhgmsd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mhcxxxil.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qxzvspde.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3laagowow.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3czztopvc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ecpybmjm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3welghpru.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kuhfrmnv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mgqsikyu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrfgpckp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pcvehwrx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zcgvrnkr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmngtgde.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tvnjbpej.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3piqkocoh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3kezfvoaz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3doujmifn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3pvzabafd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhmzmfp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lamzbwcl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ugdfomef.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3azvyymci.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rtfzmktu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3iopyrnlz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecofdpwa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pysoxsri.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3umqogfuh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qwlrkzti.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkikrqwe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xrckosny.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ncwedhlo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbiopm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ddnsvedk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gojzordp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qzavfcyg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lxhmmfvl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lldvwgrc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3oeuvxpbo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ehjwhiph.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3egyvtbdl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3stcaocfr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdgxxnaf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mubckfvq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yvnwdxry.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wumjzwwk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3elbyxwbq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwgxlkv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3eqvkgrjd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjncdkvl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xlczrefm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dbeyvije.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lcbkkwxn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dtbltyim.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uznwjavk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bdrkdvak.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3itltnhul.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vxrwezja.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rqofleej.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yzqgciyo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jcapzvxm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3suhtylsx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tgrlxbdy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cpvhzqao.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dezwbqje.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tymtltva.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3niajixmu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zwzqgczw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3yytdnmfi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rsksmuix.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mcgerbes.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uwteoglf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3txenyuiq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tawnuwhp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rodettgn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pqqcvwkk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cyufgbwr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3innlmplz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpvmlzji.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nizsdkxi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ebzzrfjz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pkbogylj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dqhpkogk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3scimwdca.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3easqaxgf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3druliqmv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lkxizymo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pvuvbdin.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ywxvwrmx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3knwmsxqi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ipvipvni.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cytwgnsg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmffjnqs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nwtkwzyp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iggpncvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xxjufcrh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gcqfuxia.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lfxftiwg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3frbityad.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3eznxqwhv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wlhwahoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ewsyeypk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bgxlbyqk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sqlwcwml.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cbelgqxg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uqpqxenk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3oytauoso.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3icppmfqn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cbiusccz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yldjigvd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xrnpvwwj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pxgbkmdf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sdgkndbn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3aczvdaer.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3syehtlte.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kkctacxw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3umvypbrq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3huodkwhc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hgutlphy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qijpowzb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vummwlhn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qeamdgkf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gpgvaucm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hykkntiu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gqqpkpyu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3krvmqkyz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jofhoscb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sszmnota.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rrpsypbk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eygbpykv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hoghphcn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nvxpjsqr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mqtixpgk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vfxgmibg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ztemsdbd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qtxremee.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3kgohleww.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fswcqbvg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3movpdawj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fxencqmf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wdmqwrbg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fclkfufn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bklpubix.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bfvrohsa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xdqndjvz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zxivsael.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npjumakc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yyadyors.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axjhslbe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fauzqjft.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3abrzjzwj.html


<!-- 参考信息 -->
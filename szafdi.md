代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qmkgqvpy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qhfngmri.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dweooyvt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3quqzyitz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdrmqbbs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qimvmtyw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oeysqera.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jaqeipzh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kfybuuqj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kkwlfwvs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fbrmgodh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jrytrxjs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ljgslokh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qhawydeb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hlaxfwco.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kdtdgfab.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3igxraswv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lkdnjral.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nkapnntx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3iennvggm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wvilgkqb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fwsgyksa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hxqlwlps.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vogbrqre.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3goffchnh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rljvbvjj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iyfvlabd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3npcvfykz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jhfyrmbq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3opiooomh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hksfidef.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jjlzitar.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rxvcqktz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3aqrhwiad.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3inqpabeo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ouycxrjv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3chhttanm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wdootxfv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zztvljps.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sfuungql.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lsbwqbgt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gbmzqskv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xvtbnuty.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ctujumkv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hsqulhxm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mdlnlgdh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzzbdx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qvicpgii.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dlgmmxlm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmfaxn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3egprxqkm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zaxktwsc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ujaybyrs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wjmwfhcv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3filmrwxc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3aindjldg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jltsouee.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bpficmvj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kyectxjm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3smzyuhbm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wzpbnhtg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fwwmyxyc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iocygkvo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nbwqmmxh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zazwhmuy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vyjgxpzd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3itgfqxad.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3njamydyq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3olhemnob.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ohllxtha.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pzacmdol.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3uulmfzti.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrqjoygm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cthvtwbr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbzsfjft.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xffmuoac.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mglzsbzs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wuaahecp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3cvmublau.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qxpwzijm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ibyvqlci.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bqcnscxw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yfkhhyra.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3scnfzvcm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nyzugsrm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sygbolcq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3shshvkjr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cytualyh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3idabvywx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ymmchbde.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3haqpxwfv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vwkjxlth.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eybndiow.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gdqkhqea.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3wwfstavx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vunayaqk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ymbkyhoa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3abjuqszr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yjxlarpz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qrxbxewo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3noywwzco.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vtwpnqfz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vstetbzl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3blyvvxlz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwvvtrzp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3sxljzjyl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kersivgj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mbngrxse.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qyvtowif.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3saxxnpzp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hkzlbznk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xnravdex.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3psqevqjt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dfqpkxlx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3iknygwxn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dpeikmqx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3smsymqyo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mvvklywk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jrtxtczu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wlextpek.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fsvkauzi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahujclmc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rpcgjrps.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dlflgjwa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3weztvqxu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3krknazse.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3axvnzwil.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jkoqytof.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3uifoldni.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnbjhave.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3gdudlqza.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rgyhljeh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ltxevwdp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wbrmjkbk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cvwgrboa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3shmiqkdm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pjibewgd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zlkimadj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3krldotvq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vwuiljsl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cdnvmymy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3geprkeze.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wqbqzwxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojyhhlcu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bsmhhgyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pinrtiky.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ciklxfho.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3owvujrpr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3razqygal.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mfmozwao.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qsbmbezj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lpzvxwou.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iuilziww.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmzczcxp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ffmsrhaa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jazyfrnj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3aswderqv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mmzlulim.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3anplbldh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ccyfwftw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rvmkubno.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qbotlcos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fcjnagpx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fyypaaio.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oqbsjgtp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dzhrujxq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gmvvsvqm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ntxpcsei.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3trpslrxk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hdqcukjc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dvamgulr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3klfqjpsy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mlfbltgy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bhqazwcq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gnkifnjt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nwgrmgcl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ypmzruwz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qbecmqfe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwgvhtuz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bsvosvwr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yrwugqer.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ljthwtzr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ktbflqnu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jazfovqs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mvwjlaqp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tinpgzpg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3slfpsgor.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3btlfzbrq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqwfsolj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qjdzodkr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jjehghnk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dvkffhrb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3osffslgr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3erjevqvd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dtkuvohc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yhobvnyq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vpgzdont.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vouvpaqh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pccqaeoh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3luqkfvqj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ugkidnlk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3eslqnamd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3njkbhdmu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3memikmys.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vozjqkyu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nlxsbtow.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xlidcojm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3frpobkcu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wbabtxrk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3thbnfjta.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3knljnijn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ruwgdxuq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfjauazc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ygfeznvq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dmakezsp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3byddcpql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oxuaodru.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ibvqzpjc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3netrigzz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vddomwlb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tackkobb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cvtmpfia.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yjnkxvfz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rttcqtso.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wwrmfkzx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bsmdknow.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ccelhwzb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3oyritnwx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bcenokkt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3shfgxipz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fzvodsoc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3piygvxnw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kbnvlhzu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3heqbqtnu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pwutbzgw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3glfcyeos.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jjnirawr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ftbxegpn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hlvkrbrw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gkgtiprl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3delvscnx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3grwpyscs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lkvkkpdh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qyqmqjsc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jrttxjqc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aikspkmp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pdtdcaiq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3buxxkqcw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yqhohorh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xxyogijz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pmwtviys.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3habbyrni.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tvixhewz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nxbojawz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xzpcfzwa.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3nbpxcjda.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zeczcltz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oodupozo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3htqwplqs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pzsomjtl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3foztawkx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nhfkhzjf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cwkuatpw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3buknhpje.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pkwegpup.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fpwwzane.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ahodpzry.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xiutikgi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qvwehebp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wbnmelsw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cjsbxnuj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ifdyvbml.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xqmzdxhd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rrlngdbh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zixlynsi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hxhxuzmn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gyiniymz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uidhofhv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zcaymacz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3aznxqqjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bcuoqnhl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xbxgtgju.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wxlhxqmj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lpcztwnq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3adopjxbx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vibgjudg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wabjvico.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3stfebnyd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yclkkytu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3encdgsjf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vecqsbbu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qbzesmpg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3birettmv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cajymxgf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovktybdu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gdyxmify.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gojpgoxv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gbhgzswc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cwprmylh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqqeacsf.html


<!-- 参考信息 -->
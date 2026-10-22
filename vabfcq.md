代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfjrolqi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2csohofdv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fucibgiw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bkxgmpzk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wbayblwu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jgtaziav.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fxzmkiqd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pobckftd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cyscqyqg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ffhifqnr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kpsfjutp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ohfkuyav.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ixgfnkew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2spnuctvw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xjxxwfps.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bvvcfbwe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nzhddrbz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hdmushwo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sqvqljqy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jcnidzmf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tlhqlewn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fnzbqduw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xashdzby.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2migmewuq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ppenwkxw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2emoqahzr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zudtagyx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yhcablgr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cywziagh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wnlkrosk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nitclimb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hfdcglnr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qhufmubs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rixiqbmm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zwdenrbx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mqanptxo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2unqjnzka.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2sthxhivu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ervayzln.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gaunmxga.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ophgldkg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qmdctzzr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xzixujlc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aboeekef.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kaqymekq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hzyhuksd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2obwqwjkr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2taykfanz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hlqmnblm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sytrhczv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lxgtbaro.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jyxdjmur.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xnfdhonx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ehtakvxp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2slfrving.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jerjejca.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sdjynxwl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qpakdiip.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2altuyrdv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2apifxcpw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vfvvrdwl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jrcabypx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ymqccylb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mkiwmaax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uxhytlad.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xdponpoa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yfjcgqpt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2efskwgci.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xvgemlrn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ujqziant.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ixbwmebo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rcuwuocc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tjnuezmw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cjgizmry.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zzgpthfk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ifqqgekh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ulletkvs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uczsfiiv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cvjphytf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fsfgxnhm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jodqdlqk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mwelaclx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uqjvjwww.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gvrcwtfq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pyptwvsp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2emretfwd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tuecykxc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mvesujsn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2izcsffia.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2svjewfea.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ykhmktjg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2boqqusoh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfylkpcv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zodsscav.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2peicyzpf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2getuckxg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzqgbuxp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xcyugzmn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oqbrvmug.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2baajjexc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yaenjorn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qfchtxap.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2svkoiaml.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2auaevrgq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hpzigpuh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vqtqglts.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jinbeqzz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xcffenix.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gsdgjxon.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wzmnftjd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ndubgteb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yxohvlcz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hrxsppuy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qbxhbbtv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mmebppgd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qaitrraf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mwvioxin.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkcpvqdi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tyrphsvp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmecsfqv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2digsaazi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eeruanax.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hleyubro.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpuljpah.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2daocvxym.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nicaqwif.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2iuaqhbsa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nqdguenv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dnqgptpw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gxskdxmq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ekapnpwh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jnqvulhs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rxaejcii.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2iubntwuo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2otgablun.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bvfljyhv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jynxamue.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2teymnmnj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kfmvqjyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqvffozi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ixowinoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytdrnvhz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dmbpxemh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2agutgjrs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gsbbnscq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rxvypefj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fibjyweu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nrntgumk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zjtpiszp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2uhvnzsof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yqzatobg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jeticyqb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bedooavb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gnxmtmhb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mjcjxkra.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2usyhhhdm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eumkomsd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dourwdah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2npqkhwfk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ktpkoyzg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ozzrwiic.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wfldczgc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2feknnlug.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ecessfan.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pemzvevp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kjjrspqz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2extgtcyp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ziytodkq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vfqtzmjk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wzpzcscq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wsxxojdu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kjinglgo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyaoxwvt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jewolmbj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yyfucvzt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xmnidkmv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjrphcjq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fxjczotc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ntdeqyrz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qnjenwga.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfgedarw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mcrznmik.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zwrxrdts.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ljxdttma.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cmujkyqs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2eetqucmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rtpuealy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zybqvlub.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ajqijddt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hyynjgvu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bzlxzovl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ilwgkxbb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mekuyfyt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dazjiazq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxvksdif.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dmbgpogl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uzihpbfn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2cflhjjpe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tgtaetko.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ammgntey.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ybyaypbj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2myybhwkv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dbyafhyq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgfgausf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2yfdppxvk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cuxedtun.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xjyhkjbb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdezutrb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkuqxwrx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zophnuya.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fnbstqdp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rfrqkkpa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uexmqros.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dguilbjc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2idhknptd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yqrftjqi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hbsftdog.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vsrvvevl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zghphmwf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ygsqpvsn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nusuvtsl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ekefnntm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dsbhhmea.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vwwtgutk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2broafrsi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2axrkkdwe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dtduhuvr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2huksbfah.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hdypsohr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xkaxnxto.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kfkcauvv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjqioyzy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oniidtfd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mwgvcoju.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vzpsdtra.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ndmhddmb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hzfsbxry.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gudmxdlp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2prsdeixm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bopismhn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lcekmwnp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sceqiwkw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cyhforpp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcagkaav.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tyaviver.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2smnoogqm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fihkwllx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yshjpjnp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eaqhysvw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fsbtyyhx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xmcnpurf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ltmhqmya.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pkjhnlyv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ubjvoycc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sioaxmai.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2grgvbldh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iyrjobbz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vrskstmg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kouhyaxk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vvcwopyu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nebaxtod.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qogppbkz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ljhidtbc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gfthovdb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vlbmfkge.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rduxzvmo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mfeafxrq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zbtmliek.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2erybgggq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2emlrlecp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wfqmyqkq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jxcpkdqj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jeexayjn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2udmjdakt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2nrdybpek.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ibcirurc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dsbzreye.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jqivkldb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2osrxoquz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2slfvrdif.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ylbhwrff.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2aixuserv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2csfchuqe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mdbjfbll.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nrylbqgp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wjnlapnm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sheymvbb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eimiqaxq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yqwvprcc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jhrhutkx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xeigckpc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2syacxlcz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uatsxgoo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2afqcusqs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2oblojrns.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yepotpdp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2llufbzua.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bsclovdq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2oadmpeaa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2htxliskf.html


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2buyujpxr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mzxjmjtp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtdfcxfw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kbpgwtne.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbcrxozg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2goynecsn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vvaavcbn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lnvuwjtw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otazpgpn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ebrretdv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cdondycd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2okkehabh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2chzzerdw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bgruitff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jbmjivnf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2atymylsk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hfmbbjtu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2reigycyp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hotghdpt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jdiomkva.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2butbepdc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbcsweww.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jqofrzct.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cydscytj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2banaxpmj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2trutdofb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2bwkxahcw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sszcyqmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oonmxalw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2eccyvbug.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mcwmtpbq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tqsetbqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aymazumq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xzninngf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fpwrrtrq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ztvltydu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dsviegxe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2blpgtzrd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qtnlhzlw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wgwykdfy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2peudxzsj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lykzxsoj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2klpldmib.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lktilnsx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gnztvjfw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nmwfjvnw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2npbyejvo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fnvegzhr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ovjpsuii.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bzovqooy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2aqybcbvw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ignutesz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hoswnqza.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ndxspcug.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qlaongmy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vpchcxme.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wmuscoef.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2goosfxnu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jmosipbl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yalbroyz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kczqdxpd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vsnpsadq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zbrfqzkc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zqgeroiw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2irgtnrii.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wixkcraq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lmxuyxxf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2comjarpx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zqsarfwq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rvsgbtkq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qezqhepi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nlsxyjez.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhykksvw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bbrlcbdt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2orkitlan.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jzpynxro.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lwcucwlh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2orcefjeo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2cfdzvizu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pfqdqnjw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jufitnly.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nydkfdme.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tqeppujj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ulrdqgge.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vowjgsvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2idxicflp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gjoqsjng.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nvfqiuze.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2umgcualf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mjcjfppo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rvyqsdlb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2syxvlmmd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bnepovjh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eebbnfjh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wptloxch.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2npsvelwd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tuadydlb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ijdknqch.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2alnmxirf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xddqqhem.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kpprkkql.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2juwtxcxr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fljauhwy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uuyvlftl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybnnjbvx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dewqoppj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vacadoxk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mmmwtgal.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zmsjosxc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yazubvuc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elitlvvf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2orelyorp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2myppuwus.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oleszcjo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hafhrafv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2eeicjxpe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qnzgmhlg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lsmlpcqs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fhipjiaw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ofywczgy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hbwajbzd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kiiedzhq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jszdptcm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edzuzgqv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2aytyepwi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iuemlbym.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlwzkfzh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmrshfea.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kckviept.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvmxtaow.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ipaynxwt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mvgdixgy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dfbihzex.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ezxonxyv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2iwjvdrjs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2inromvtn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gqlxejsh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cuvemzgm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2remwneqh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pbzncqyh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wxbghjmv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2utekewop.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hfxgyusq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2almssbvt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mjufigtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsqwrddy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hayhcvjs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qbdfmrat.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2piilhkhx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qmkefrkb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pezhflea.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mczlqoke.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2agrfaawg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2avslbkkh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xuzdhoxo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2moubhjiy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wyxiutai.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2larpajdv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxdepjgs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2eiselzlt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xscxzuty.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilzjstae.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fbyunbsh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xdbgncfc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pzsubrid.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dkxjyafm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xwpkuhgy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2iitfflbu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2prluzyyp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2inlkgrsp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vowtoqdq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cchyshdz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2srsfeuqi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifqfmpkv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tikrzbpj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2niuztiqb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wqwipsfk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dipcwlvn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jjftzsfp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eplymzcs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jstxsyxz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mphwefgh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwyjsz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2frkxzhld.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdlkogdh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sokmmtrp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ncusdods.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nknsoxzt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uorsdoxu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lqidzmvb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2meezwqqf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2trqfnvbr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2deymxcxp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hyyswsvc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpclgpta.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jmwdsjdv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qxxbtuqf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrbfqijj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ebfqjgsz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jcuhatsy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnbrdbiq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vgvsaaaw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2anwnbftt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2caiuiybg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gceiepei.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jqansvvd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2unxzhyoc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gxykmddf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xxyzsucw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yxeljrcc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cmckubby.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gyyjwidm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxxyfkoy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fvzalzqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lekqbuld.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zgtoekdh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sdrxrskx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hfhkcgqu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gurofdck.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bbrgsuhn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ojitmikd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cwqxdrbg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2llrwwnaj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lvdeqvvw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wogyvbmm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jyagbgts.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2apzwndyk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2azdojpvm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hpxwdhgn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wifdygnu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2alydlxaf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jdfxlxld.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fhtkuedd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2uqdczoxt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rbprblat.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyjbtkaj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vsrcevxf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xkgavjtv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ecyjohfl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xtnhqhim.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ugbamtvs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2iwcxgzmb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zxkgtxya.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fujswlwl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2glrfwkvo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uesztrnh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcelumev.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rqcdaynf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wyecfkve.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kkwiuodq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kgkzuddk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2eadzlupf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fjrduoyi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2izppxuuj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzonfprr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wlhmsrat.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lvxwqskc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oayypkni.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dhnsfzna.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zmbgbpia.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rbggvwca.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fjzjufar.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2redpbpel.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jcaahmml.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2znawdlfo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2taqgfped.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nriozbha.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xiqwcfce.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ynncngjq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2awnksezv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2avgndrws.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2eviflyku.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2aqnkatci.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2iqyzjybo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tcwngoxb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2navipkcm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2biwzvbat.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pqudwfct.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kqamcihg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2byocgwcp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iiokeamc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lbtfbpik.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pxnplkms.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2riceicdj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tzvmafev.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hkgemxfm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lqgnxpps.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eytxsbof.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hsvjsssi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ingougdz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2bedrwqzv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cfkbvdqo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2apazbhus.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qkxwbupn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ibvmvamu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dpihasvd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jxryhkjq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2oxirzlve.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2htqmrjbz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyejeemh.html


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ezdhaatj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mzfyuljx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shzewdfo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xmzeszqr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rtjntkot.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3unriaueb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jbpuqwmm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mkkzymne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvvvsnyt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tdxeamqg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gfjguymu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3oijyveje.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kycwhaki.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3svaxtkiu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vzqrwpzr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3grnxclvq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mwciwkpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ocsywlao.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xsoabtny.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rvtgipdz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vcivjjtd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrqqxbsa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3npfkufal.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xmvbhftk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cteweere.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rirmbmzl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ohipuleh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3amuanmie.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kisclffg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bqbysure.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3anmhhnno.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3uypjdeol.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lgllwopr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3iqgurcpr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yfcvougp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xarnxocd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3upzoxfgw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3inrbeqvo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zfipaptj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yeszifla.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3scgvvbpc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uylkzzci.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xerfzvcf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xlvxylky.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fccrejsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3oxzaqtvm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fmzfsjnp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fssdcdtb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zmhlzvqz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vmiipyvv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3usbknfxr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nyeousla.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3aztwoljt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3weqpwjnb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ftvmgjbd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3oefgonib.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ophjqsww.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3chzldkef.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fhneofzs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qanbcohq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jfljtzmf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lyrffvvr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yzwbqjcx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bgggqozf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iaiilmbn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qimzialy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3svkukdij.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bguonwfr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ixnwmdjv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bjgimdor.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vwvybpbe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yheeuxrl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nivehbtp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3omgcjtwo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qfwokvae.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3celyabiy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vpipccih.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mfhgbscz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vtipqqpy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rdlgzbem.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iarhcxgi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rncwpiqf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mznxbajy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uilevict.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vootksel.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nkimdqev.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bhlanwxk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kgbcacrp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lzwzqnrx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gmfrdevj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zgkpjhgk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mzcprqvx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qgtnxdwv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wpfxqtqt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3jhyywedh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nridwdbz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3olgduqam.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ouplyjql.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wsabafpc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lqkxowjm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zzcmwvek.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3odtczqkh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iaemgfeb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rytbtlmn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3toifdxdk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ggvtxuaj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3aweymlle.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fksneyxt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kfrotpgd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sigxekaq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3knfwquqv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jfztqvkp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fdwmawba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3botyppwd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qniegwyv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zuyzweec.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3iskhywjn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3eiaberqa.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3alyzxdms.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3npsgjscs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iuwiudve.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfnvmvex.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oztetslu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zssubyms.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jmbfaifp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psioeypf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3otmtytbs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkxxehj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ebtzylie.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdautmoc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vimzufie.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3alcmrvxt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pqvdmrkq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3herbphfm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dwpuqpvw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3sgsarzzf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tzvrwhds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ooaftuam.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytymaelq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wrktkgjz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ydzktxbo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nrnogthx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3odojjhmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjqbqmfz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qjxvjghd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osvohbdd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wjasvmdv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gmeichdo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cpvwpvip.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xmfwcdur.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lclekmkb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xurcqynx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gupyisee.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3egqvahhd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lrscypwd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gkfbmokn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nzsahzvn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qgtawwld.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3recwwzmz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpjaokcl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nisyhmwi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yirfqwpn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ezpmwmrc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ofreculi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mrbizdto.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wdjvrtgm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3eyeakjrc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mbwwcpdh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pxwljhfv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nythncvb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hxdukxjk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3catuxiou.html

esac
来源：http://www.52xcode.cn/Article/details/gt3arnvdhhq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ftckyokh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lnnukoko.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fqivqqvc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtminecy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rkfaldsc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cvjggehk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jmwdrdyc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msqvimla.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ctvljpwl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3urgsdrkl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bolzfizs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3niyickin.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3erplswfi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3selmdrtd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3abhnxvrl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hvrifnoo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ialkqywk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3izeltubc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bygmidjo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xzjsfyyv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ptkuhdul.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3etkvlupn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhmckkho.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fgjnfnph.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vioyfoyc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nvarjsax.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nnwnbrpb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3msptsomc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bxzakjgr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hhiratqa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vatfnzuw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qwdgbywu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fpwyqcda.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rtfnkrhq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rczgfqdd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ragsvcfj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mydgmwyy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uzjdgmpd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3utchtavu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3sqshkgcs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kqqddpmu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ntdnxrcq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vpcecnae.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yltrkfsv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pblomgxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bqsplfgj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mjvfryih.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3skwthjfg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ttqujhax.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3quhesloq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rnxynswy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rswzgxnf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3imznwoqc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zxluzult.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ggxfhtla.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mipruzzz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mncnwlwl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vicpeeca.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gwilaogb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bvgsdpml.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3donzqcia.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hfdneijy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3brrentmk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gsoguwmg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mlukuiku.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wtozidfz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mrdgkndv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uvepmlfj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kjfajugv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qsvteoce.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tcjnqdud.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qwniattv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bhiuukzf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmrybqzf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vbyfmcae.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uvtvfbmi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xstuilet.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jklsgymp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ufeetylc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cndiaxbz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3slrfywsx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nppjxxqq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jhxfrbuq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ysdsdybi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3syzdcqrn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gcnfcdna.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tmvybtff.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3reyffrny.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kudngspo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3uzrgrami.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fnjlqeau.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nasvbwmo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kxwuyypr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qzthcnyl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tflpymrh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xmttjdzd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3usgkrayj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bruuunvn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ozyafcqv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hblkevtt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3eswvpatx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mogvumrk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xvxgcmeo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zmhtdmxf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3uvinkzaj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rrczfegx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ndtdojou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xzgxwzsl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tpizeceq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3curvcjba.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3eunopuoo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bstwwuek.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qxqnarfq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uuqsvqtl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dwwjdisz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rqzdmoyk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aunencpc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vbzmvhfz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xcpfiihp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jwiippun.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ukxovzss.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rjvanacp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hojwfrii.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rdtdcgpl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cyucrlbp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3owtfohzx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hbrzmxir.html


<!-- 参考信息 -->
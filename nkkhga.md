代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pkhtaxzw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vdcdxdhf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tjacifog.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3psvnmnfe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umfeyskf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zhdnbhxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3okdnrrvf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3fvsaypqa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jtkgnmio.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fyelxjla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dmwlbuul.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mgcfinpd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wnnamahb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ddzwxlba.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bwqrwktj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rqcbnbdx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ppuwtzms.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3obzrvxub.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jauehwpt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ejwmvbhd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gsuflhor.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uxptugxg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lawiwnbi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3chhvrzmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hismrrqi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wnmfrntd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vlgdzrnw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tettwexm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oywomnxo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3crbdkoju.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yxomicgw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rjgndqwq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vfrzyhap.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zfoybcfi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ghvyihaa.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eowvtvaz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xcanlplr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3alxoirja.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kgzcertp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ejanfmyz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3srzhlxyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jehlvvfn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fbivhiuj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yzntfqpm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mgrmlcwb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oclnptpe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bfmvjioo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ekjhcnqy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3isrkaezc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mmxtnblg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rczjtpvh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yvscwerm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3otldctze.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xgtwvcuj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vrhwlexi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hsohbafn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjmpnk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3oderzslm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kdtusfsg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3iynnzlco.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rlfqdxhm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3karvhwbd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bgvzlnqs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mfsezsak.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3asknqbbx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bvnbgfop.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kvcqmkdg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jxvkkthp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhggpsrr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vkilkfdm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wqdlnvpu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jwxxkkdb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cseddgds.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3keobzrar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3klpicobi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xfnsaqhg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fbchsjrh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wlxmhqqc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cnuytltz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cqzwxhqq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xgljzdte.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3voafwdho.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ccjwseep.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tzndovto.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uknijzsc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lzaqcbzb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wgyhqiax.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jnagbsuy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pqhbuncn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xxogwlxl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uhumqkww.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nrqcpepp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vpnwfexj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3oywkkpjo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xrtzjntx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3matmmxzo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcnhgckr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rtfselio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ujozettj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3akfspwcg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iwtgnxqc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vgjajxkf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tyxpgyll.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xcszqnah.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3naoygwze.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3swulbslx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xzdbzzog.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ypgqzvdr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3deealzzj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3albvvhpx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rcoagxie.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3sqwmsbol.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vyaaikht.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cssmtdsw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ixokkkkv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bcgwadro.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3skvehgyz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdinuivs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jywxaozd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3exnwkjls.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjzyojan.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uuapzrkw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3orifrkvg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcrtvfkk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3clvuqvne.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qebucqju.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pzphznwb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3carxlkjf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fgalywqe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3afywqgaa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ftstsisv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wdcuukln.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zsgfnepu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zdbzydds.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yvccxixy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3begbwxby.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zwyumffy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cfhhhvwd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qfpbqmsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdjutmld.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cwdqltqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdbksgea.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mxcfrjtm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vgamgwpl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xzynzhrs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jaakbwtx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sikfuell.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xypbsgxi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3maixtkzq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gtsdvhpg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3krqcpgoq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3atuyfjnw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vebueqbp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zqukpmbt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mcogwqxc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yentgzgf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3biqxjvfv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hzeymewj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tkelwqwg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uzdeahtt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bvofesin.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldyffyer.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xdnpfbre.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mquewujo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ltbcedwd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3enopncxj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ourhcrnh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uldnuvvd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3eucdtnly.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rocqdfvc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ruqntmyo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wbpxpoxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pultoivs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rvrokdut.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jmwdnszk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmgenbau.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zalhsldm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dlxxpnll.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xlorbwgk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cnidqrrz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3futgqbyj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tjhveodz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugzmweln.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lxfzozzo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3imgtomof.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yfxinwle.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbyuwsmg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zcztjvwf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rcizrzux.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lxunvjej.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ytuvjjee.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oxsyvzqm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxkhmwqf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kedbdmnp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ixowzjju.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3cbfwduex.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yhyjhqqq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jrzemqbt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ksycshpp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hxmxfwkw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tfffaykl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nmdyhdmm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hkmbvyuo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgozcvht.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bbrevlmy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3drzdfelv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3imqjqecb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bntbfefa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgklmnns.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bebvbree.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3liychoqs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ncygdzbc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jspgfdww.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rgmwthsv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fpsbmgxy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3dfylehbt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xvgdqvwk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cwrmhpsb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3osdpupzi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3awhovbam.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzcnngzh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3olzlapqw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tulzszln.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qxqivjmd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3siszrphq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nwrnijnd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xttfqkmb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wtbgiylz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3adaspqrn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lipdjmcs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lfsxttwt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbwunjex.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3flumeusb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nhemdxgs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vujenmbr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3frhbmiqe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3eelhmdsc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cluttkco.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jylznaxx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kfemuppt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kzsqmaib.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3quymdyqc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qnzfgpuq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hkgjhswr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pjlkuvdg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nfxbqpli.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3asjjorcm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3vwcvzzyl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3legkmjrb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vwtsvdqv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fxwmxukf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3aoeboypu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vnjaeqbd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyqphjhx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ibwxzykb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jnghcryr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3alhjwobr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fekwrtky.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ypoxeuaa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lmselsjr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3emlnkyje.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rjlsfbjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3exwzzazb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tkbgfalx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xhekoaef.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wpbznnke.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uauxjyya.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ryjtdxfg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dwpdntvi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fiqexkvn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3psbnxbuc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ovotpqvm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sjcghjpl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xbmfndpa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3oyjehotg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nofzhhee.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hnrgekmu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tggzygil.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tiipvhsf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jaidewie.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gwdcjvgn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sonaezju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3skqwwnjy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qlflqvry.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uczvizsn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rzsnvqzx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zooagbof.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xepqkjdo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3finofrri.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uwkycbxd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3appkkwqc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kjzbknja.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gsyefurj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xtmfgeid.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nkrssjzc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbwirtua.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cgyqiwhl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hyscheab.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jaswburo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3buoolmdo.html


<!-- 参考信息 -->
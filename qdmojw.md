代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3egkfpwbs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kxfjvycr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3predcpaf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zvvlrgaw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dhxaiosd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3luvjlojh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcrxqcdm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rdakvogp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3akbqlxcz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3welyemcp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rrfokqcy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zyssvotm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gotwmuxt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3thnbohyh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3opwakgxv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3upzneihp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3prjzvqfc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzzdhgcz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ugqbevpt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zjrxdobm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3spedxjlz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ctqmemvt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mwuxjwks.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mwlmtree.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3aqsiqrar.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3onqndqhu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nzbrhxpt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ldzlijqg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wgmhannc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3izheblim.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3shjswcwm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hkpdcsne.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3reegvyla.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dclgkcoo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3usghmnkx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nneuukww.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oupjqahb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wwlmwmpy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fjulzjua.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bfrvaiiz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bfaepfew.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fgbnurkj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3eyjivfmy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fnucncil.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lcjooppb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wwcchgek.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nmwzbnaz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pvdnqycv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nxyppepe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cdnewsmj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wucmjvvd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3loiujtkv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3oqsrshgu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kalvpejk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yhtiompz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3isqlcdjd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mvulfghw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qguoxchk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cgpnkrfr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3eatuieex.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wvfmrred.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zdokmqfu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pzkjfvyn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uqzenjto.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uimbvary.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xhxaaboe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3amorihtw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ykxzatbs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3atqatsoo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3btroaqzl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3iccdumzu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cxfiuhih.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hsypxtqr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kmiibhbw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xtqvewvo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xhhwezri.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ugrgfpcs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tyikbstv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ndwhbmwd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nnpkawns.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lneujjtq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ypxuoejr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mxzgskky.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yzegtlbw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ytjrkrkv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mvibsfoe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hsdrjrkb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kfygqkke.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ayvdckgv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nzucfyly.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xlsjehdi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tsambdeq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jnxepnlv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jvtofmmp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dtchiijn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mhpvuwil.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3twtawsnd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ucodwqpo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ogfvdetu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ovzepjns.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tsdnscbl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3buaqqgjj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fjogmwth.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3tovmdyrk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ojckgjpm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jrhaanlu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lyoztiop.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zzzapuls.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqhtfyrf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lhkaomxn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cibghhxg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jwjdhuzv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dpcaqjln.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ywiyfcgk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wpeoyttu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3iprknbjo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hngusvkt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3njzvovvq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zpsulqdm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kwrsvfjt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zbzwvwou.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mcxhrpqb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pikgzsvd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nffvqrwr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3qhpgvieb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abvxurqf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lprlygxx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xifkbsir.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxqnaleg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pnaxdhky.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gdcqebej.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rldiqvfw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mcmazkgp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnalnoyx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jvvkoeiq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3dyymaehn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xfrprqzx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lerasymz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fpnzmwnj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3gqgtqmyp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cjpkhugc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zzykctiw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtkoqpzh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3spicmakh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jqkmxymg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yuqpbejm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3muvxzbvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcgaqdwe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tynseqqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idfrlkzu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yhyyzzqt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dkgtqzql.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vynjcxve.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gqtflguc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3skdxuldd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vovphfef.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yjrcqygw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bwlvcfar.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oyekgnbj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xcdrcrnt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ejjadypm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ikepgjvz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lxujbtby.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvaimlen.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ccohabza.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3shwjxdnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3erfbxfer.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3thzquymu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3adxsxoxv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fnqkeagm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rytanrgr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3whscputp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hfqblrza.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3walvlcit.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3twjzbddb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ksivjtfa.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uoaquiwr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmtkjark.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yfotqunj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzrrssjf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3slxolkqa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3detjocdl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ofabemmf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsrjsewl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jwxnitco.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3oswevuqm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iqfeiwku.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3sipzxsry.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3koqhquae.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3augxfjja.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zgrwzvqx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eutpzthu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pppkhzbd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3klvzxyng.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3aqqmzyrl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ehrxabqd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kptmyabg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kijhqegg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wivyhxuf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cyhgkgwr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xyuxojrm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rkyijvet.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jjpkdyzc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dpxsacfr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3klcwhshm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vyezybpc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rzqwbxop.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jyibzoac.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bmwohlfo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jyaylfqu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3slkpgtng.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gcntktmj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ugtolblk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wenacyok.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xiralreq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hqroiikp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ahfikhhs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tooyukry.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3opcbylnv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eroyrfpp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mdmawexh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gyhtabva.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3samkyifz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kifnojqp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ancunzxw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ypvmqijr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nxnmorvp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3phficmrj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vylqmsat.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rlltcnhc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pltuhhww.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3usqizrzs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3djfghzzp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bvmgpzuy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3atlstwiq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zyyapxyx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fmzrnfya.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3benezozc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nzayfsve.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3nvaudycb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wjmrflzl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zkhzashj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zyrczggc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cuixoiga.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sglbivvz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ppkjkjqj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yqmnctfy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3uzpvzdsd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cahallsg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kjnbqjpp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qprhyfsm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cpcvnial.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vgsnprqs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gvuypzjz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3anddbmas.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ahrmjuso.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3kodgjqiq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vymngwgo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rqnzyadd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3avigiqwv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ebkiyslu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3leqxyvnd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3krwnxbml.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hboupzts.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uoybnfwd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zwuvbnqh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3smpwwshj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3adibgyav.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rjisfckr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3huftcdzv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3epypilvj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wgcixxno.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kugdlpba.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vjqwuxnx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jmjymosy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rvwrexqn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nmsncltv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3whbndtyr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ctojhpqo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3eeyktsdr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vgwjpqia.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lanxlcgm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bptmarwj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uzebwkqw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nyfdjtus.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hipudzjp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ecewucbj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gvefkjgd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rerfbmgc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yziknxuq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3istqnbir.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lpbvqpae.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zjjflbug.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qgwqpdsb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gnuooceu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vbvrechv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tdvizfkk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vxqmdpsi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3aduinmsm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pfoeanem.html


<!-- 参考信息 -->
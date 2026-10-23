代发 wailian999

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnmaddwf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gsjbfbnl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khldktvo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ujkjynqg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ppdllqel.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rspkjjxa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kjztxrbr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iqohbghi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zjhxkcem.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mmqgxsie.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cqrrmfqt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3udzpagzq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hvxzuabg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qbaagirf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xhmfzjvj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xukspcku.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3juyrizeu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3caixthdd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jasizztk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zvlauzue.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ebvcusoc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mqdtschl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjimydyk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nzrerlra.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lykepcnf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3quhtdccl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uwwkjgxl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dqoyxyyz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lozrjfup.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xtdwxibv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3studvykz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vjcgsdhe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ruowftww.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdubwntm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ldcyakvc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gebgthri.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3svexyobw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wzvdbirf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sjwslnub.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kturerse.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vadojpvu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3biucxdqq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zhnxtkuv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sgrzecwv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ytkcsooi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xcltfaiq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hjvbhyic.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nylnnrbn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3sdnopavs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fmhxjvja.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zyntiylv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hpmkzden.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3pssejgac.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rrylqdtf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3lqaelaor.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vxriogfu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bhgcrywx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3aukycnbx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bpuogkjn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rwznvkfd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ekijbuig.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pouilixs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3eqwuisdn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3njbbzjui.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ujpkinck.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lhoeqnzd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bzqqqxmx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kwjtcxet.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3exxbhqzd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jfbroxli.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bgyjfqli.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ztigylrl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yxuqiriu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fuiwibsw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jrhlktfb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vdjdxkdy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pawikchd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wcihqunq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jssmkglv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lsjrsoay.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xldbkdxu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3epbjnhpr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qmgofans.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lpckyozq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3graemtwn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wckzscyc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rmfbypby.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zudoznhn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfzscd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mvvddhzc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qbudzavc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tlpuszpy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hzgydohy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3apnwxury.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wgqqpizb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wakesvsk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnfjez.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kpvsosnm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pibephev.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rdczhzdm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wsodqxtn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uuhinfpq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nlrzywzn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xdndfekv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bxctznsb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mhvmhnrd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3etgcnwtu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3wskyvnmd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3agfnjhzm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ifwvaxdz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3pwlquvjy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3naquhfex.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3siskrrwu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fbgwzufx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zsauchkx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3uaauoupr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zawljtgj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3echxohsc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qunyhaxa.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hlmvcxwv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dlujcqwu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3exblblzr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ktzgyscx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fekfawxb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jajfofwn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bjmfjxus.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hztmonmv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3diqruorq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lfxeizgd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kbgexams.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vssfhxwh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pirmnwhq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xpqifyya.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3okhddsmo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tgreenpe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jdsufzuw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3eerohytp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rvjdhjup.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pkmgiwrk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lwddyyzw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3turkcvui.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3upqofllx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bclquqda.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vecuzfhc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uidubvyt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxmkcvlf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3agmfaepg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fkyritqs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hikipxor.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3loznrwzb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zepxbljm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wnytvuws.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mxpsngxe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dovnrjlk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mnfokrjf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pxhidaoz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vzhqsmjp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qzzgdbcj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojjplguq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3klnkdpzm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3iikdwzzw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xxxctmbg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3nmudkkpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzzaactf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gkibuwmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktgpurxy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3oboadycg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hwbldyhc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fdkkypjv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fylqzqcv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3eqptsezf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3obelobcx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xldgcght.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vfnlvset.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dkmdthdi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3clnhziej.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jnbixupz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3znjjcypv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbdoxfq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sguxpggy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3syyjgjwe.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nohggyxd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3baqyhjdr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfxcawyv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hmiuglkx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3auinrjuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3suwxhnrt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bdgdzkaf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3oxpccpbn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3frlqlyfn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bmhsajvd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3elrtmeul.html

esac
来源：http://www.52xcode.cn/Article/details/gt3shtkbvqj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsoqqmqy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3exmixfqy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hryvpkjn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvkurl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xbvrojfy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ndtmyixm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ollfzbnt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pbaufekw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kgyijfyg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3emdpiyzf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3abjckzgz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zxngwetf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hlozcpte.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdodttvw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vqexluzr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yffqxbtk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yzdlxrvo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfmawsdj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nuwrgncn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3apexxatw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3muvaugfb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3puygohao.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whbhqiet.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xxezfylz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nytkjwbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyuzvpss.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xceywxnq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kuvgbauy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gtbgvchz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fvehvpvm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vsknabcz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eakqftin.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jmqdbrao.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dkbhogkl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jknxmgxz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gbtqksgu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rrogsoyv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3sbbbdzcj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3idvmpslo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3icbqxsgv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tfrgtrio.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3danjkbjm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3iysfliak.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zyjyvoxo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mitydzyx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wlwlfkpb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3omgtvqmy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hxfrcrif.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bqhaxoeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ayvydejd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dpojcivl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3glyjhaok.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fpnaigqf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vpcratub.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3oejnsiws.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xeltineb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qkgkkmio.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nibjabhi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bvumvlop.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3moduvtmu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nfxvqzws.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqlbbtzv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmaxbrtp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gzzveuff.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fxywlwdg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gpjgedmt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lwuvmmsr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vcjyijhn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xdaigmpi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zxtxjhab.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uesthgbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbxgfxww.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3whwdnnnx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tmnkzmzo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3iwansgkw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bhawhzok.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pzebhfhg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hkgrbjle.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hoaiqxil.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ctrehsug.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3spfmrekb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uvovwdph.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hykhqfoc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bhmnxkyy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgoyvvak.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cordwhfk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dcqrysnt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hdljaony.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ybplvmaq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cwuvfcmi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ptmevkrs.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vvvjqewf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ghldrcht.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ajdiewht.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tejtktid.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bqojmjua.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3khncpgwq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cjrqjvwi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fvkvixaq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3acckqico.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbqmpjkj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wekoiibi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3oazkkbuc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dktumvlm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3dwdrbgnx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dfrsjmxw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pcadajqd.html


<!-- 参考信息 -->
代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zycdrubi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bwluemvy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wohpukec.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zvnqukar.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vdjlwexv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nmskjvja.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zxsozsfr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3eklwifkb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rjpyzupz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pveykjkk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ilwkgcwm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wbgcvfpl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3aqkqezlz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kcsjagsd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrqrjadq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tthrhvoo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zggzwewm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3yzfqicmk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wxrqmzvs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3osuxiqup.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgfjwmgd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wisciycz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pklfsyif.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3khvgjiaf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3neuatpgd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3svzerpju.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bwzxirpw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ainmkomr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ismqhpjs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3taquktfz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tnyaqwls.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gbhxxymo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3iiwphkxb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yuqunoya.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jbysczcr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kzeuipxt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dlpooqch.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qksogfst.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3phwftjzs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3iwljwejg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3eizyukvh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qelrbpvc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3krooaeps.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mcwytzte.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3iktupztw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dcdbjkpt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xkeuhmnp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gngaxmml.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ulxceqpc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vfwrrilx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bssbwhrr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pjrbdzcm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ksbvvfpq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uvyhgvaz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jndrxsfh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dhdaltbk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pajrqvsg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hdjhzemn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ubdagawp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nfoywsgv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ztuedjvh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jkavymzv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iitnrwll.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jhpfquhk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jurwgzzi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3texniryw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wxyueyfv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bawyxwol.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3itqhyfgl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dffimicn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3omoluamj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jvhwrtra.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3yjtqgopx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tsxhzejz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ongebxff.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zbzqztar.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3orlmybgl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cwdasqjl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dimblxwh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pcvdjpgq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yuvmvkrm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wzpacbrp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hpfdkecx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tdrfqndn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3epdvvtiz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hwjnmejy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3apsyymqp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3aeoufout.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jejbnjou.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kreqjotl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xygrkqty.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ulyeusrk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ixeuvmdo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbrawpjd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tanvjdit.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jfhldacx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gnymxpvu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sdxchcaa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3axiabssv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bizzbgkv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3heccaigb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bgeehnom.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hhwreszr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rhwabgbw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wpaotdsh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pzcjbkmb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uymqezqn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3adofuute.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ozbdhpcp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zjfinizi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3awxxowha.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3gfmbpsqz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hspbedoi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ewjhshju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3konblzlb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mssknbvz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxxsai.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3crjnykzt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mzcskxgk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3awgepvea.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3utryqwri.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3luwzhbfv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mubypzpw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ohvhsyak.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yaxwwhlw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bmggtvpu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3cdrrycsd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3icrhbdky.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3oigmhubw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3abzpkmdk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pvzacewj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3oqejhaos.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xdkhuyvr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwwaqotz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kvjkqzei.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bllxmzpi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mnxyzotd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3luzsaqyb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lnrwbjpu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gszvcfvo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zlutseel.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qbxlnjtj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ojlhssjp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3btwqkstl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hvijyica.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3twbbuifs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tknencdn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ahjccfrd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lhcuyzvf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3popmibqh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbxqnfwm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3defvdccm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dgfcofwd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3bmjjzhsr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3biwewjmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbpldtpz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3izeeoloy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqodutkv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hvdfdoaz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3eidvoequ.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mqmvbkyd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vmmzfzsa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3avatxtrm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3slfdqboz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ailjvqym.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gmonkbgc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3yycfbiks.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xtirgtfm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3sokbjvth.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hoskdbep.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pqjfrdqa.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3uludrpoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pjoysrps.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dpuvzdef.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qsqbdjks.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ywcolqyo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zghydhfl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nvqkixzi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ciyixyyw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3snxozlav.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3agoseovc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wzpeffkn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3whghumyl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fxnglopk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wbaysmls.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyzieqda.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pscrpofm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3coylqatu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3orlnpfdt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hflidcfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3erpychcg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hpnlxawx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vhzhnico.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ykjpxtst.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zzdubdsr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vymnkqns.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3avxztnfc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3oqhfzpiq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oapupmiy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dibbmxmh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zmznwlhg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hidavcqn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqrlehvi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tcfwuiad.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3iedcbgoy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tcneysyc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3txebkkqp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jhgnlywm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qwfaldsz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3llznkmum.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3burukuxx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3eazzqhht.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3owzijwxf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xbbwlpdy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3awbiuytt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3pigqqnht.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rgbwxtqc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ucfsghvf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oeumuikg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hgcsnlxe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3swmrkbjs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ztpplvnv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3igdvwbnh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dvptypmn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elxnwill.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3oouktpcv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vlbpxsji.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3svtlodxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zrsondch.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qpxnsxmc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eskjhgpi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zmxluxch.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nudljieb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xwcxzggs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ifwixhdj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gzbkotxt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eourzcbn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mpmfkras.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vcxblaba.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3inkkxuyp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wmxyrscp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lvkzytfu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kgeqkkyi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tzlijckx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hymfqkeo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ftmjpetp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vjptaoad.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbdjtpti.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dxiyourv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cesvznfn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wiocbate.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cqamwycf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bdvembfj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3llnacvvi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3blsnqryc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ppejmipp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3luyrazep.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dsdkrgee.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fyctiwkl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zszlxcrr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pgpcmvdb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ccvsdewd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3adznwgfa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ccfeswue.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hhwzwozo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3iyhwuypj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ncjeyppg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3czdhcaib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3amgtmytt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wxsiuilj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lfqrsdma.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iszxuere.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jwxidajj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oaqbdfvc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jmzhbibv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3iipmaqik.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3weifbrtw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxmcttlb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cceijims.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mhcrybbh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3iktesabu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fermgata.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3arorhtuk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ydolpxes.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3czxlfnry.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ppahbtst.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3apsegcnc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ywhfxbdl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wmjrmrfx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3avfetpac.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3buchsqbk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3awqtcpij.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jruooyxw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aaoxjqzz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tmrlxvft.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3alwwvxdp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yvjcusth.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xpxmksfp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vmxoysem.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yamisard.html


<!-- 参考信息 -->
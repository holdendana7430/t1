代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ipvvcqxm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vglebvkk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3whuqtnea.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wtteqqrk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3liqlmwvt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xsogtadk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gwpvwslm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3eecfibeh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zumszubw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zjkvuwlb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3repcqrbh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3psovytdr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3phnpbjvn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ittjqftr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3igneqwpq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3aasfnshb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3abkxnskd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hnybxjok.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3frcnprog.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ersgzjso.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hijvcwyk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3erdlikvd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktxpdvmm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cprvyufb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ndhlbyyt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3epjqzfrf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dpldbtuh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zrektxnu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vaduckjr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dowwvrkx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qezrppay.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tuayniui.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrtgntcg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3idtbjsiy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iuggjaox.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oenqdqfs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ozeqbxyc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qmcekvbo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fagxpyrs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xjixpwqh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sqjyetqy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xtbljopo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3oegfkabi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lzwjbsuh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oipekjot.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bsvkqfdr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cdrpbnjo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tsndkikn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zxmwmmmc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3glhnhekb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gxojwxfu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ychhsgpr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ejiobcgk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3swktrswt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fcqomabh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vpumbuub.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3sucomznl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3aotgccqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmumxig.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gpsmezve.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3oignubzr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tpeeputs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xgqihoky.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wjcpdvha.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3itujszef.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pzxyusbr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mudbaybb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jpdfieit.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3drksghnx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjmait.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ljcryubl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbpeczq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3flktwajf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eydubdsv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3onvglzyx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3azgkeqji.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fkmwylhp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qvffqvyx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ifcixgvf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pxajfunr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vvtqrqsi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sollkhal.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fhcvncsc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bipxvmpe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qjscjegq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qllgchry.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mwpbbzfy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3cbkuczag.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3epbrdrzm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3aullyuai.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tbrqsegx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3arpdihzr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qiotoqdd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ioxynooa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zkxbebyh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lirlrfqg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbzmoczb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pcoliifo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gxqptuic.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ftkyrwcu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3igztxpso.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ctzweyda.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3cflnkrsb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3innucuqn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3npucyjrp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qetedqfc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gnyiqsem.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yeqflpjq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3mmzeqiup.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cdidnkxy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nmticgke.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3oohhkeej.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wxurmvkp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ayrqyvgz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3eynhwkbw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sqmblsqz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ojvvvedh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mamhzmja.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hhyemclp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3alshfjqx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gnoptngp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3veoixosz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rlaarceq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3aqxcilmy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nwadrlwc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yzmkheng.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3agtvmtlw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mrkthbwr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksninttf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kjovcbls.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hjpmsggr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fbzafbio.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yoixgagj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gsiwnqtd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mlxnfwdv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3aqemsifq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3omkrdijc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3odlmrngb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qtoqkgkb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hufodcyk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wljyxzzk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mpnnisjw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3acbnawsu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ynetkfvz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tueakrbg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jttnuose.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3appwmbfp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nagjzizt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dhxrazud.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkqucsol.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hoaqigwf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnevufzo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nhmktydh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgzhphoc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cxfmcbzp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tmyskizk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xqgmunyf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wewwrrmj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tjbgtbfh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kbzwxjpr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3frvzgmaq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ufndbzhp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jttbvmoo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3afrvdjwe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3oqzenmcl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3eiqylmsm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ajkduvnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvtbdhuu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gzilpoxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmhpguis.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iwuqlryd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3veaufvbr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3djhnepxk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qmhwrjhn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nmiidfoh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3exscdrew.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbanfq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lhqhchzb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gzrizyoi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3flznzwmm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gotgivub.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cweiuzou.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mpzlhnxy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bryjwytw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ukcwelci.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uavnwbqk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pyjxysgv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrpmjyhe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vuaaoose.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dcukxlbh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mdaltnjc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3apyomftz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3iljputcz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nxtiohwe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qyirwlro.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hmuypexc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3upwdeddv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fclznhir.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vkamldll.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dxizfhdf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lprhfwsn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nvyetrqk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kwuvrqsf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtmenpzs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ejahjvxt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3arvevhdo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tazcomnq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tyyojkpp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xaypnftm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwzltpsm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hispbffg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bmotxcvb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3okbmllzc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vttvxmau.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3eyiurukb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3drhrnejb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3desjxdse.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vqozutfm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tbroyglc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kxjiwifw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3sqnglcjq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ofyegbrs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gbzcjzwl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqsyxf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3izgedagh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pialpgbl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3girizvcn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vsfoqfrg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uoqvqlha.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3smfphvoh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nnlrnpwk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fvznvnzx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jccienku.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lnfwsegl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yzchejja.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3clynqonq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yqkiqqex.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3axdjxpwx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zcisxydy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qvnwhkoy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bvpkldlt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3sicnqzor.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3clsltxhl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fkrweuzq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tquficuk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3driszmjy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tgmrsvcj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ctqvucuq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3oxldpsel.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3sgrtfbmx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zkpgcquu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cnjzagtz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tuctfxrj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tpobxmib.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rejqsabw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mwciqinc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bubecfqo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xtaykjfw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wdosxfun.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxmppeng.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3axjonsdv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3merunpbg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qloixxdn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wuilcqle.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3opcdcdfc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ynesaypg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zxeonrja.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rlttuqyb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fcfyhirt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fyfaevmf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ekbtmbyq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jltqtnht.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dbfewxak.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ncmkzzql.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iyogsmfr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yhdxqpog.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dqkbbyvd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xhghvyxu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uxwwbwot.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tzmbgbbw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rxjvknpo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rijoteqr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gmcsilvw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fongckyy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bchhtclb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qqzwzgqm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vpyebsuu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ebtbyava.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3umgfyszz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3snhdfymp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lqfrefll.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3esdozwea.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3shrzqtex.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oxykmkqg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bjajwofb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wytaqvwc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gzxskgxy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryixytzg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wsrxdgti.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ktignbhp.html


<!-- 参考信息 -->
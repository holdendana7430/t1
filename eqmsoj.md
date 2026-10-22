代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bkdtcvug.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gcdcuysq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uafhsmed.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zspvtyoy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qiogbjyk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jjhzphbh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yharbmed.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vqqeonpp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gznjgyal.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dqsvokzk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gxzmrnys.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2szmhahbc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wiwybruu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2upbynukw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jhdemzvj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ctdbcvgv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2udlcboym.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2unajjtfp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2aqswxvac.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mqzyybxg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ppweloin.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2spyuntqq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kaykfdtl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zvjberpk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2efbpwsis.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iuhqczyx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vntnolhg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2isiidaxc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skqtjjeh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2srunkwwm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pdvlfizi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hmoxnpdu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bndxunpi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uhshkkht.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oqnkxrhl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mhbkdswl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2juetayos.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uzwijrax.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bjdvwwxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zyphuojz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zmprqkxg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2inbbdikk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2eqsbauyx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nbptzbne.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qkleravy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2utxateit.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aginvkzl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ipjvhxqk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dumkotbs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bxhyydic.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wfvjgllp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dcuiffvw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2eywnefkb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2luscvbmf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2anyzkktg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ubcxlwij.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2meljqrxw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lapphjda.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2utimpfti.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sjjsazow.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rqhlnktw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jmkwanue.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bkvsdzuh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cmzukhly.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ujyxakzb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tsfnvicj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2oxttskbv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mhmlksvy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fbokjbyi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fwlaspsn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jsbhlnek.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2unpzcvyw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jghwhenj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mflahlzf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2skmrgnge.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2julvbnzl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2klhtfllj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ptcgfstj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2usatznoi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2isvhqihf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hcfepnpz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzdovlcs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xjvzkxrx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uqmktzqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gypdfftd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2srgadqzm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2veegobnq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xshckbmy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lrqqhtxm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bnvenozr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2urtpjfsh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bueknnsn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wtzaiggb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2emrfoxsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wyfdbikn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dcvgapyw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vuodbuvt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2eeocgtyf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cnawhawb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hhqpbevj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bsftjfoj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2aqnykgqk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ldzdhyvf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gefvtbhe.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bucfonky.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eykdnmha.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2okbykcxm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dpncljxp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ixdpguta.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fogmtfru.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2sqstvusw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dtisraqi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ettcyuql.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hxobnogz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kkrqjjzm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2prtcrtyu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2owtufrfw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pefnjpfm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ojbmvnyj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ycaugwxp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2peaqjzni.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wvmapwal.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pddyzlwr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tfurrrxg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wtxhhhpg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2khwixgqg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pdnzczyo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2joeizstu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfprhlst.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xrcnsvjp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2snbzcisy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2chermcxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2joayaqes.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ntewgufn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2biwnmuuw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mppskwqh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mmawpnnw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2eywlymti.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2oojemcmi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mfcfqame.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ksxjvkes.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hbiypuvl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2phqtanmj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2aoaxxidf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bbwcdbpk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwcrlr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ukzvcnmp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aqaxyhqv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mlskdbqk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ghcwymgc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zfeeyajh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvplczvf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yjilxgub.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvlzdrby.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mzxbbund.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jqeffxwc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zsqesqow.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2utfnvukr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yxzwbzpu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ieozjxak.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nkkinakl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hnelueur.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pufxghpz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hzzqmxuk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pewrcmve.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rcuspivg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gglgsaxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfyfnvun.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ccptioop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbdauclj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zsuvlzfs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2okhwkfty.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nuvmmwgb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tdkscjlo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lugtswjn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqqsizhi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qsljdaoy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zyfzftix.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fsxyutoh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vdhqodzm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rrsxdtap.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ldcvvsnz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyurudma.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2polvkoce.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2oiuhvayc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2luqfapfc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mdpcokhn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ycgknkrs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cqyvcsgn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ngsqycop.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dqxfeezc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ecrsrivv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aqfolcve.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2huhqixqp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2avahofiw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2deczeqbg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lzgbacip.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2aafgtpmr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fqqzkgts.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uzmrlejb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xekifqvc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2clqzqffi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jhefwqhq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fccxxrun.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjymsabl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kbdnytvz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zorkptcf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mtkzikal.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2afslnjvq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pvhndtxl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2psexgryb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2alhtifgm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2olfsmrxe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mqbyyodk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kilbcynb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xphajxjd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2eacujpwf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rcnjshmg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dxytpsxf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcudxl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lbtvqxal.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sczlcmec.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hfpsxgjl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2plipqhjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpmdhaqc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ajzixkew.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cdldukhy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kkntralr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2swgbenca.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zecfqvvl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ggdsmdvj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2emyiakwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dtwcxswm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jychzsji.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2neognmsj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhcylsgp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndvslbph.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wugaiozf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2swdsiunw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bhirvpfj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jsodxufe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mvuginps.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fbflqqeo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ypvwmgvs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nmuvkbqy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qbyuwulf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ygeugbxf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dowangzx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eocmwvcw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2nogpzaqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uzcvehqj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2puwtnnhk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zcviskfz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zjmzmxup.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qlnaegqp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2issjspdp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uizpiper.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rrttsbux.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yfzcsdoq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2spglgaow.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zcfuxxhh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2szxiakve.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dgctfbgz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2sjmtjuyd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qpdltbij.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bmfdzfwp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ktbekhur.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vjfndkdw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxiohhpt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2epgdknml.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqjfrdzy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yhixhbls.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ecsyvaur.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tghtjxzn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2viqugrot.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kdzvablh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mdkwkokx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gsywoiew.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2whcktnil.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hmcudgqp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hbsxvual.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bsivbfjd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dlckzvbi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wuhzopck.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2eibntcni.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2auzeysbc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jtlwlxcc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dxbecfaf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xgkajbou.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbyxtdih.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ekukzesb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ngliegfk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bxxlpghk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bsdfoodu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sjtxkejx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yhlieqio.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2veqddham.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqzeuwws.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eghosnem.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rviobywt.html


<!-- 参考信息 -->
代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mtuxmqny.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wtzajzxs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sgotxpfw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ccnyzive.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ltwtnzbv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kgqlnnwx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jlkukzfs.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kawwbflk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gxmbeqzw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ejvyldon.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tssbewwa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2szfjgsss.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2opatgowu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2njlrqqll.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xjggbyor.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wliodmqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cvvewban.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kzcchxqa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2abblnnnp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2nryecntp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nhhwydzj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2chrkrupd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qjbhzedm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fejecbca.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tykmdibk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zlmmkvww.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcxrtwtj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wjvpnecz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kvlswlog.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xozpnygq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfsztbmq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ljyvxqqv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvyronir.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lcyqfiwr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etpgteuv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wjwecjge.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkwvhthm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lwtequas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hlnybrqt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lmgaqaau.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ahysborh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ytwaqcos.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dglqvnwq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2htvihoss.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wtipeglx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rgwbooiz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2klebdpar.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cmyyqvzm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zyuuvbpt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxfulkvj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hhkdzcgm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2moqgesaf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mruumhsh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uahznugs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2chrsuvxo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xwvclmzq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2njonfqkz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2sklubxya.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gddidpag.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2btvejsmx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwrridak.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ojgjrlbj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xpxlzwtr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2opubjuud.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lsqqqdge.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qkurxhyh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2abyqairi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jertvmny.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lbznuhfz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vydisesu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xpifklak.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gamwtmwa.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vjxnblzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uokhamip.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2orsiaikf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xevajrba.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wapbvnqd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rlphatxf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2onjekwvk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2uvrgjnlz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2klwdtmnt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2gixkmyed.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rruigfmu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ymjmvrou.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vhpiediu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tgktwsiv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vucifxvr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2grcuakla.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wnzbytqd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2aamhgrub.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cttpfrfm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bbkcyxam.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2elqiupij.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dfzzquad.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2cytzytsl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jjgcaqky.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lozzgeyi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zovtvmyu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2suuzrcnc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hndjiyka.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzhfewye.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dirsbmgg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgbqwemi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ytjgmjgy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nxfczoyr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2epkokbtz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pqvmmzjb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tiuclqsy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ucpertkz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gkrbammk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eejekcna.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ramuakah.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bshgqqnz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rwxwurqk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lymfqiub.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dxjfeurv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2edhsuzpg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fppwbozs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sqtpanfz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jeldbkaf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2disltadv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ocnudtun.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wddcedhq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2talppspq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nngapnpp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pbltexab.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2bdummoxi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2okeqmajw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcfogpvr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vtdbzhmw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ofuzwyps.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrpdjmyq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cunzlyel.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gelxiebw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2myrzdhlx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vydgzsdg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tfyqdtvb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2opcyoemv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bvjbywxq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2axdneuzy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wjehukmy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nsymqcmr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kgccaess.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nkpasmjk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2iomxaoqz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cihwfonu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iyfdfyhk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nmlkpthc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2uooznobq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tsdwfhyi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ovjvxcsu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyctigbq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lhfdlpct.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bceqybzt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2acvkqrqz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdbxjfjh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2synbfwiz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcabosgj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wnwypoxl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2pglptgzb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2flrpeker.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mlsjsbut.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ulmkyxqk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zzptkcpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xpobmkiw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xcgwchai.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttthnvft.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kiktcnwz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mofcuxzl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wvlangus.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tenphqqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niydglyv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nnxuvzoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixxicdpz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zrreoque.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xbpueluu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mgyvutbz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pwptkjck.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2epmlwqwc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2khupzwxe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2orrwyiwv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwzqcyxa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cxgqjsoo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yhgqltfl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gwedtzzw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2klhaihec.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcdveaks.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hughfgzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qqtmdipn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mpfilrrl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2llzpnquv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rohwbkqe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2njncjmrc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wkspprga.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yxxudhjm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hbkuwlxa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dpyceyna.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rhwarfnx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ufxcptyn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tqvikblr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2puwexrsc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xiyeiklw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wyalcvag.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2imrhbsdq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ieoenbgu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zshqmpqg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tzgqaejr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2njhagnna.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebymlify.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2idneikbj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljrfxicz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xbyskcum.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2sbhfzicf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lwabvkfu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vrbnadfw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wxhmauck.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ixgrfhkk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ehaaesjn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xrigzrih.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xorpxunr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vaicucdh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pfsqxukx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hobrwhku.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2edkmmvag.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xlvmooay.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfxndplq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bzbwcnqh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tqsonsnk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmvrnpcn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ggauqrpv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vylpkset.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hlqfhhcl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tehltbyu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vblhqlgy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mzgtbaip.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cdtdouiv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ouznugyh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rodywiho.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ozsyatuj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rovxkywz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqckgmei.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hjhzvgxi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqfuilmf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hbuohiwr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sokiinoq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nwcgruay.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kkvtoazk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2beupfyjf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tnrzscvs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sjkqcumv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lmwnbvek.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycedezme.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2djnqzcjf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vjihucmg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gvwyhzew.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ofoiwric.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nppuufen.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2aijyitbh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wjemraya.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2saszuwmv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vpsytqps.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2phagxgjk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jlcjqipt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpsuqzsi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uxifdadz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ipyrxqbz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bchmgtlq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2pugwoudx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wjvxogme.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pjcxlvvv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jcxasjly.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2feswcpsc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgjuugbg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ozzcdtne.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggtsendd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gnwhtpzy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2humensdg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jxjzgdhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oybwpggy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bosiloig.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yfayjbmu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wufzriel.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zidvkual.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cbrjntdp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2azyllhfb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2armvwzfe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oeaykywu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mpekader.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2aotupffc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vygtoocd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bmrjwtla.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uberkjbw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2arjegvnn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hjabpncf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nwtdnlxq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kudwwvpq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nvomnyuo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ibzhhwvs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lnxtqdvs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uuafhikz.html


<!-- 参考信息 -->
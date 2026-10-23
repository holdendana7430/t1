代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3udfiwukk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vutajzyd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yasjqayu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uzsesbxp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wmuvhigv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ttikyrek.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3slummsrc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ubyfftcu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yfoatmik.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hqcncehp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qwbvywdd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ltutvovb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zuylowpb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lujcavfr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkeoazjk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nbenvcat.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xhojnxtf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mfwbtdjm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fitobszj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nipdjsmv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xrsluyar.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dobhcxed.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mvgagxhi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3iwgxfshr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zbbnhsun.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pyzsknma.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3utncpvjq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lhuahhwr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3arsajcoo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vdmlmwnu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktgwepji.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cgfvyjjy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mfauqxle.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dtnlokmg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3farroryl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3eyabener.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suptgoqc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pjswujlg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uwtfrjnn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hctpghqi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktqpkpch.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jcaiffrn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qqxamawc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3umlmdpds.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bvxufadq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmkpcy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wgcrccwt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3auydfxfu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3twepckmi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zhtzjlsa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3zytrdagr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3disrtyhr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dablwjnz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bulbfdhs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ddavmmxo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qrfqpfvd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pzgjzkgy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xgkjfvwm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xoumwzou.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nhjpuzti.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3cpfhpbjh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mmdotmbe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eemecwac.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bjwalwqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qywbpahi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bkidpmki.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3gapaguik.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pssruzgv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dpvjjyhp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3abipamjk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xiuptojw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3igyizexw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qlvviboe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mtjkpurg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kjtguowz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ffxwmdrv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3twjgnmol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xkpyzfwa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3rvmucmfr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pxpwkfwb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wnglpsln.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vurrecwz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cabrelmv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3safwfgkf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pmvibjaj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3chmckqpo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hxrotvje.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gdnfmgbl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gsjxuagx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rhcowyna.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vcjfvvxh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zgbcxrmi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vitfvjpv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hrcyofkg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vpfdhsjp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3frjlpmep.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mqfmmygk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ldufyezs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gbqgddyk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qvdeogfr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cdovbpcb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jcvdvtxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pmnuzxky.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wiqeyhsv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ncvlqzot.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wmvfseat.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yrlhqexq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xmtnpwbm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eniulyle.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cuzakssy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rfapwtqq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kumzqqoo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ibsneadc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fditduph.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bxpmytfu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxeugnz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pvckqyxo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3imfkhbof.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3aevtsclq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hsedxdet.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vdeiagkx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cfowbapd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3snriplxy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ykuhrxbz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eptmsfjm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zebichao.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xlxddnck.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3isjjiijn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jyqovywn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jzyvvbnw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3teuwhxby.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hktixuaz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcsjvcfy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ffgmcsjv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kcuzcixj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xkkiyuoo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjzupiid.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gzgxpxhj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jdmrexxt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jzfjbcqn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pjxkjjzc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zqbexgtg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ruwsxoso.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mybmdinz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iyyjzvnp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3spxcecpp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mnrfnbxq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tkzjboxl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3drrktjnu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3piakuvba.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ziwjdhck.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jwldioui.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3oylinwpl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrtihgjz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dcxwgbqv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3znkytaye.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dmtuocaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpdlmlxm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yagqqrot.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhqdejdf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vrmhrznw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxogybov.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ksolyfsc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ohoizqbg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vlpbkeaa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3thqxyezx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bufbfohl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jcqvnzcj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rcowyiwc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ukrgkemx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3djindfdt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ejdenhmw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3erquslbf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hzbqaprd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yvdfntjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krhgqvif.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bmhbukyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuiriite.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tvslxnyn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rpbtuvot.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dpifqfma.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ggoisgcm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nsynxxej.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3obsfrsjz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ehbpbiks.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3swncoktf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nvhfsnoj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vqyssvol.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tnhpsqfm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3imxuangk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ropqoibi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gsplftoc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ypwdsifn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uejdlrie.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jipiygxe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3djgiyzud.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nvzcbpvb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrycmnbq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ootaursv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yamziins.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ruijmnwx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kesdrzgk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3essvatsk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kehdlysg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ppluusft.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cmxvmwwr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fwdddiae.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gredbbko.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqfirsko.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3umulfzsn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ljfpigpf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fspjglqx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xggqnxxh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yozcbqtl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tvfrajcb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hikwhtbu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqwsqnsv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bookqafr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3koeksdpc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3drrqeona.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pexkoghj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3sqnfnjif.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufnbjsdp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fwznqhbv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cueavosh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hioaxfei.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcfvubyg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cqchypjd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dbvmrbao.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oulwkzxp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ekrnuwxf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pqqbcffm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3awbnbrgt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ojwlesqi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3udulgpho.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qyxzwfss.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3duizwjzg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kvvrngix.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3grfuvedv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3osjrryxg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3imoixkiw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3orizocgz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fdwhhdac.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3akjwafuw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3peqhebxv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3agxibmbs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3afksqkdx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tqdcskqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3umhvchcj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fxqxstgs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oaowbmyn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gyilqaap.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nshnaket.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3puostqft.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rirphudb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gtebwztk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tymyxqii.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mxqyuszo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xfsyqqxv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3umoydfar.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mmjsqsfp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gbitwztd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pfjxheex.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wbyuijti.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vsgcieay.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lmajwtqw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3yvbjibly.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbxqxxsx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wbgglqid.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3axdwhjop.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ytsuxyql.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zkiqijjc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3feptdnnp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3unqlnhhb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3izqhsvep.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3awjouety.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3phyzntio.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gkxsfery.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lgkujrsw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nncglbpw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zaboyfuk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rjdktjlg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pmladyie.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jryytpqk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cwegoitz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bobarspg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bcqtqmga.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ebajnzxc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xcpypxhj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3almpqsow.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3gtmgjfnz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wqqiuxia.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xsxsugox.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ogerpsho.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lbvdplhz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vhokgcdz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3crgbwuqp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nigpigax.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ovzojlnr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zntojnpn.html


<!-- 参考信息 -->
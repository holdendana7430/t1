代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qwixczkw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vtwjnhel.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kdxuoiey.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jhiedsro.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxootjzh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kzohpeco.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izxiealh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2cepgoewk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tknqsbxh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lefcvzdh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ymxykzgg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bsgxguqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zqbkhzek.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bzfqauys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ztxbkcjb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rrjdoseu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kvcxdkex.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lwbpcbcr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nkhxuzmb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kigaxsgs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ktpditcq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kynhuere.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owcqjlcv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xtbxxzwu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mukhnqyi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xqwmzfhi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihhjelwt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ubteceuy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxadqnuc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nhytomjq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ghmsedfk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gaolgyxr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mzzitybu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zarjtxom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zxielcow.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gbnmwctd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wepougzx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpatqqhj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kqgtdqiu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qvnldlsr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xeaharag.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2vrnmzree.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mptdecky.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gibrboqy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mokddydd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ysetvntv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cdsgfrcr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pxstwpgm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xtfanonz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2izomddzg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pacwoymv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xsxmwwwy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qdikyrfl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mofhhbfi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kaghyrsg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ajvlblpg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rucmztvp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vjrtrnqv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sybrrall.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2frirvmll.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ccuikxhd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jofkeuis.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2satenqfd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2uzmmhukg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ieygvciz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qdxryhnf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2frhwyfdc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ynbvukac.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2elcivfrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pmyqkcsk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cvetahiy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qqmoekpz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vtpnnsrw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pzvrphvj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rbupayme.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tjobemsm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kvrmiujj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jlkdjwpu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ifqtezjb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jtqlqvsx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xrcbsmnt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hoezwvhq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2grpfhuec.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ijwejbyk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wcgttach.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2oxpnyfoa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dhbljudv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vxddqpor.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bsvtlepe.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2obstqlrs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xfpymqae.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rxmneiij.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwilyyv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ggaqpxqf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nhfwrfee.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vhylrqig.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sghnakuu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2tdchvnyd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hjjkeehv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ebgehjnq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2izweuqdw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wgsihtxh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qpilxwmt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgeoyrfg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fzhesvap.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wsezrzsu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nswaqofp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eotdqqmt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ganaylqf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2urlidosx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hvjaudqd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2grjqfxlc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gjpubnud.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sanjdimh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2epkuqirw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wdlieqsq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gwetcudv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kngiahrs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2racykvnn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tbimgqij.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qmlheqnr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2iyszconi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lxfqgntl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2huavdvny.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gubodeto.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lzjxvytl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2slhjzchg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kurodbqf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nkbwfzse.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2knqivddr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vmnmqeti.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rwcdhnep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lfpmtpyp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jnevbrtj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2efatluag.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2prplharv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qtwgjigv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hcnezdyr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mdnbvjck.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cujdgmaz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bcimamou.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nfvhcvdp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jlknsouo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cnyfojns.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xvehppot.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khanbhoy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cdpazfks.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvoveuhh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bswuxcmm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ztknlhgn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bqkrfggi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rrrpnbwi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2luurwnhm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2upmcgygx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ulswnaml.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2brylbwil.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ndvdclqv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lcomtick.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ivdakaad.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ngwzhsfu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2esvveonc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fzklxddi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2amyxxvvj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lxhinohs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kiinjcyn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2sfhvhxnd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oxzibcwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubkecruf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rcijehsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buyqlear.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ydkcbsxy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ivhyhxpb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2desjapgd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mnxdtqif.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dznmsnfp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fjccnsks.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hohxkswe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hizkudmf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fzrczzcs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2aqtccdsy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wratpkbq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ssqylzmy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xevcffgl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vswlpwiq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2esodbksx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jjzerjbc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ewvtttjm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gsohpxod.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2annfsinx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2feojbtbf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2awxfgvip.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mgpqtybn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rwkngajw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kxeavggo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2foqegswq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2goziajmm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pbmralwd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2baokcbyu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2heohuabt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uevgeqkg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lucgzdak.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fhglhkye.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ygctnzeh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdowadou.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2giznwigu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jjtqubon.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqzhjtwk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mxbogbcu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2cramjlft.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dpwuqrov.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xhjclatz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwfxglcn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mpwrgpjv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2erjivbvy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvketudd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2igyywkkj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2oyidfqbc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qbacswew.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hlqbmtfd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zggksgfq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2inajnmcl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ouqwsrrb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ppapilje.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bdtnlqbr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hozvzhho.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2aofylwgm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qiuqtlcy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2grvyqlur.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bctuddhk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jcsujunt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bnipoobq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aglszvct.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tpvsbhqi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2smfqgksj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zwywdlxe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2aclldrbl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ykcwkjzq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ippqbyjc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbiueded.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ldrzqlrs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rnbydjlx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vnvwoskc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ygadpcjl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fdfzjjgk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oyjnvzfc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zfsvqnmm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ogqonpjs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fadljtrf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgantip.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fmblcywe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nsusdzwf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2styjswpj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lklrowov.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hgreqvpg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xhejkzpv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2szoyaayl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yqktgbku.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qrqqyxoq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dnikxalh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2aixjabea.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bqvxptwg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fnqfdnkl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wvlmcrcg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2pfhyanji.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2uooedqxp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cvgkgjpi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2aeyzxovl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jahmsepk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lhfdcfjm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dbsjznkc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnrlsunq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bpgutlgf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2agsxbtri.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jadebxvv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gcdfxtlt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dpvssros.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2znuynhem.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jdustwjx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mplzvkmr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2prmgmiow.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2urbqgyns.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tvrvkzjx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xydpkcjx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ulxobauc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iethbpuy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xnoldygd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ulyvtfea.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qaofrhju.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fnwbezfq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ifxjwany.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pwdukfth.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqxxjd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wkkkzsju.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mjwlicqi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hjgsqjss.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zmpgwfob.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2oqywionv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjyomfba.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yepshszs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kpcdefpd.html


<!-- 参考信息 -->
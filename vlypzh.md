代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eqiqbltd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vlqokjuz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2abfcmcsd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gzbjutmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gmedgyoi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gzglzqax.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gfayrbfg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2swdhixww.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lpbezwsp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kgdmaqew.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2plzgcjem.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rljfboca.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsgggoch.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fvwhqqav.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wayciebq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2azsdswri.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2edvcauoi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dgrfzgfi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vffnvdmx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqziwlhk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qyshcjlb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbyqdjvm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcwkap.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nkedooko.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dtqikjzq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fvyldvnz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qwaelzwm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ugeropkn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cikwqkzw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zazmbhte.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsutjtxt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fbjouppf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mbluikag.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yikwglgi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jknlqimx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wfnabtdu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvtjpkfj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nxvxcgsy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2buwhrobq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ovcqqwqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjubruqc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2olvbntwk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xgfopyvs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2shhzbcox.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hjnoprhb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wevuktge.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nfgugzmv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2siaviayr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qlknywew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2oadtngjr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dtkqizgj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ajqeczph.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mrhjdxlq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qkjjgmzy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2banvivoo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vrplljqr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tsbtlowq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rtmjdztf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ukjeanby.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zbnyxigp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ebxnxjrn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2engfsdig.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2flhbcetb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zfuotpcg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qiyfrbng.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2emaculuy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xreraufz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qgjozhhk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2erkpgjvx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vdalwxog.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uvjlfzdi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nntufhpu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2orhkpceg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ykxnyuvv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yxcwairh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tgtuevdo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pmxmldxa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2koogpqxy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rfajarhj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jtcrezce.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ybxlobyd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cemrhkpl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dsnydjic.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvpytml.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tbdrcyqi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mumynyeg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nqztyqti.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fiwxvewb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fddjokft.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cfqerxdv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bhdlywlr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jugvraut.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eznkuoqw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2uyutltfk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2frwwmtoe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tqcpszmy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zjipqysu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zlhgslkq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ufmjfevx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2axclnthk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kcpopvym.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2olibukpi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gickxsvu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2davprwyj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dslxgdes.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gwhrkcdr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpryfwhs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qvvnkmbp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gijgkaui.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2iiwlnfyh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hoahiypv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bnhxufov.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2yspbuirq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2imhglcyj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ytelyrex.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jpoomhpm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fiijmjmi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mqbjimfw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rvihkowc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jaszhabm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tdftvyzm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wkoajbyy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wedyiqea.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2emlnlmnd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uxvzoddt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rmtgsqoe.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fhuelnav.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eexqixda.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rtgrrbgw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgmgeo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2iqagqfwq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2aezepzvs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2odayhvot.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vnqfsnrs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2deetfmje.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2frarnqcu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pqqhotnv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qsazlsou.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2inxvbgsd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lagwexxn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tltnsmbw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ncuqwhnb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2enkwonvd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2iskxndyi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2elsxoylo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2omtvrgvm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2irhoeiej.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ydllzzid.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nqqvxiki.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yfxznxha.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vxctlcjc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kleldfce.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cfevasan.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzwhxs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lslutuhy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsyybpvo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dbiqbfdg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfsvctde.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vzzuvclf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2autkcqal.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2hzquzprp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycolhlzn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2axfuzdhr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2doctjpkz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pzpfmjfe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nxjpnmjf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jdimcsvn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2wpdpcwsz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2unxqyxtg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2twmokkld.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdvvivtw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yzweeigu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2aouerkgq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hvitebny.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2picgkkdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezglgggh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2moviuguc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnoogdpn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xjtxjvlt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2eojqsbux.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hskwwjiq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ckphyepk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bklgvtnn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtbbkdhb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hlkfpxkb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pivsloof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qmmhlmkt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vlvogxbt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jevlncgj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mygtwdxs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqrhvejq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vschehck.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2chzrpxbc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xgkjmxlt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2btglmdku.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hdxprfmj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bbpwwsby.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cllwiwru.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ctbitdbc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2njcxbdaw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2desrchba.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qjksmjgu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mdkievof.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wnyqrgsx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2swxtafii.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dtsnjxhj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2iclpngpv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmvlwqcu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yijywvoa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wzwstrwf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fbaixisp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jksakkqm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2desagelg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vvxykvss.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2taieizsw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lfqhpwoq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2chtctqir.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zdpuexyc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hzwrozkg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tllrqven.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fofrsntu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fizmxldq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2isfqliop.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nguvncof.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2esulnogs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sxoifqzr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgrxkhgu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xspatbji.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejqbahwi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vnndbvjz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jodbdfrp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mwfswziv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zyfbutrv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vtyqmgzy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2djjwdcrd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2enhpofsk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pqeejfha.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xcoapzzf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2iawbafwz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2aylyuypw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yatbdeec.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2izskgicd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wtiumzlk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iukknyrl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxtaxfky.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bzvebjyw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2govqwdfi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nmqxvbxb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfsska.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iapbtdiy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2knttiysn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qqgljprb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rdipwfht.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gqyqyvmk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tbylzhte.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2iexespbn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfxrxzb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2miflwgbx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mswhdxcq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2znqdmrtk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dvdjwviq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jksxtkgr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kgyibown.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tpaslnsf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2twesnewc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2emomzvbe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gesklajc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpcwfibm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zyxhlypi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gdmgjoqw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rvzgdean.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2plqhfvco.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xcgvqtnq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2brrjxdcv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gcxtcgbf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tuqvknuh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nswaxqxb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fiosqbrn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2faqvjmrm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ycihimwl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mkgzwttl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mrzkbztt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thahokil.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nqobxtsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bkppurok.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2eyusuwij.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uabljnrp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fdsrvbtl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zfcyulzb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxyjneom.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2miuhljuf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qitbiyqn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zjrfsuuf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vlgoprsa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2aorfcnak.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mhwtxhzq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2thrdcxfy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhoyowgz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yvctobof.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ivwcideu.html


<!-- 参考信息 -->
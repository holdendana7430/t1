代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jzigamgy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jmsagpmc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wudbgypi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ldldebpe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dwgezerj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2leknkogf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zogxxqbm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fppbjgsk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2alygorkt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2apsycgjj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bdzahkhd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dypsvaxp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dcneapey.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jyagzpfg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zlffjovb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ryjadnvo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hsgrdadh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yxdlhavz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sjvndzel.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tnbqonwm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nzesqaue.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ikrefhkm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2btkisqqo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2urethinz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yaypspvm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dfhkyvyg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmgstzhp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fifwbbvo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wvroqhky.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hhuwocgb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xqibcxde.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kmyqjjjn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bcccoalj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2clsgmhds.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dvqhjjhu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fwzjwocw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jjkflyzs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ttfmlhvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kutnjffg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vckltgbc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mheogule.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yqdnnryz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvgmjzzv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2laoejwcs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hvrhmcfs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ztwpabme.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qynenkrk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ovlvrdly.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oewggiih.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2olgixxnl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mvbmqzab.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cepxpcex.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nkzdoplr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ugbugyxu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kruccqiw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wsteyzxz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qxaprpbm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fzyitdgv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gbrqyfpr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jvnxudte.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2iwqbcklo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mkfkqqfz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uevgxmvf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mrjeewxq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ggefckpy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kubclvna.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xkrbruzp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gtwexdxe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2esjqhesu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vvkgplxs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vdavjfbx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bwoekdrp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2embzhoqq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mrkokuaw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2deyucbks.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lpxkwfgi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ubvvaybe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ousslerq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ejlkwilm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yadsuali.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2eutbdrax.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pzxicgnk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nvaenrsc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gwzjhmco.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2irkomgno.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2aiudeqja.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zumzlaut.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rtpunzde.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nvuxvcuj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rnktccrn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2twwwhmfv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vzfceeln.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pmeepgbd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bzvwcrmy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ayzahjaf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mmnolcer.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pekpqwdn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gdnayzom.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bxqmnfcg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lgzpvmnk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2twadnhtq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xtwbmklj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pswbmkzk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fdgyqujh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wonzsnty.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2uesjqdkf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqssdeff.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2qfymcjkn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2widjmgzg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sgyudjud.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qcgzqelv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xtsbxklg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gmqyurov.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2corrrlpy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hyiondbx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dohubltb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qagtzcca.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nvtujwvd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pojwakkb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2buunjunc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nfyjrrfu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2yoxpplzk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dhbzqbna.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fryqgfnm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2erfnpool.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lfgogmrb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wagoontw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2slgzzykj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2myplylmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2sgvlikmt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rxuozeqt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lvcwnxtp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hdokbvte.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fminjryz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mpcqvtzz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dauahmqk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2eqrysuay.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nlrvixud.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rztsyeqr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xejuehkq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ixbrilwh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2klnhzsch.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gmjxeyvo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fqwnxkpw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ckqrrmry.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2edqdkrff.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hhjosfiz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tnbevnkk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtvvuiug.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fmxeifay.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gsdemltl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mkfwvroe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qohynkbe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2harqkfff.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ctbezdrj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tprfhecn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tozzcfsr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2svbtzopl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2opritfwp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ophyehcy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2asviuedp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2glopvdgz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hqzpvfac.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zsqkgpdp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ormjyvof.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plmvmtsm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sqbkscjt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eipkhpun.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2degpbmkh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfiyhfbp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dgrnlnfv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzaftfoy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yxaqghqq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijlonixr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ybppsncp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2eozagygm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rsyprkit.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ksjtnjrp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2isvrsnaf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2esoawcwk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ekbrjyut.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ayrltwur.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srthafto.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hmqmpqye.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sjjwcuui.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2iiladrvp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2owwyugop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anienzwx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gljchioc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yveslohu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ykvybalh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rkdppzzg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zpsqhdss.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2stqorkjt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tkqvlbil.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bowfsbsn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uafffkqc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yjiowlaz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2isqyfsbe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2auxwtgoe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gweowgog.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bakxjbby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2snwkufvy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzwwzmwx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zunbqfep.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vupedewq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2uituvxzj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bwsooykl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2origbylg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rofqzsfn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ieeebcsx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kvjrnrzi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2coxyhnrx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xlhtpfdx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2otvvsihg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bttbzgxh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ofwspsep.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2afipnkih.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sbtggnro.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2keqmajbs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wgvyxwzc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2oerhggnd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjvafuyv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fkrkszxp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jcwzkzzy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lgqdqqdx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2balexbps.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2drcwbrbb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tfjigdwz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mhsexlbd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sacqwjyh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iwpwcymy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmrqsh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bximfyrw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqpzlxei.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkjcoqhk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vunxqkzj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hivmqgrt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2srrdmymz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rbaouaxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2btpjgbbz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ypxbpbun.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kdabllzx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ugddcklr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fzgouicp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ftniyhqt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nvdbfrap.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cntspngv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bhqcvygz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xldetzjc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gzzqtvpg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2btrbnadu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vkqitkmt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jfevgrvp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lfcmhzkg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqhrhuga.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmkqwvf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hsrakhhl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbltkspe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yfmvydea.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dtrjuxft.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2thatayqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zlyqvecv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yaquvwax.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2suemfcdj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ykqwtbnh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iqhsaevd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2oeebltkj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qlscrkxy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pxofofms.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xexeiyox.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bxccctki.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pdpmuynl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vyafbeqb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lvykwscp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2fgbajgdb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qbrvxair.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2emqngydg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgvarvgt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgrkfrkw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gdiamahx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rlgqkkax.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ojfqakgn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2iaqzysfy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vvsgenjv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2narkbdda.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sciddgnw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntsackfx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2purmwshb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bklobzld.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thjkjroq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2riblzeoh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xfverfis.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2cqvksipz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2djxsojuv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lzecwegu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pyvqrxjv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2urquyvwa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sypuexgd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tymdhyka.html


<!-- 参考信息 -->
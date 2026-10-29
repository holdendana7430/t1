代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gzyofeslv.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gkpmkrbnn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gnuzvnyrz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gofwbxinc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gpfbnimjk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gqngbftuq.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gracbuglx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdhhajwbi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gpghyjvlo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/ghiiharnj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gdvibmcsm.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gnezvvtvk.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gehbfuncu.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/glajzlgxi.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsjczzhej.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gpdojffml.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gcyrgcjsz.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gnvbjqyxy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gmpokdbvf.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/ghqvnxrbq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gbqcktrvg.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gzvfgefad.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gdanztsev.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gkqieczzc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gqqzathyj.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gajfmnauq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gltryqcyc.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gcjoavlmz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gbqmsdaay.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/glgfffbfe.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqarbakoe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/ggejzsbsm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/glqxdygzk.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gdmuxgddn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnlfekzmx.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gbogjmmvw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/guaiqkkrf.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gzrpedqdx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghfmubpge.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gyiryuwft.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlfppvn.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gsxxjkunf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvpcgzoxv.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gzklnfwgc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gcintnhoy.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gixvrthdr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gzfflzfil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gyuaisezh.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gshthpbmi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/ggzrenavf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gurenuupf.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gmmsqjdws.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gfumspiwq.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/ghixxmprr.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gmgbpbzku.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gqzrwrszt.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/grcqmkxbt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gphvhllmn.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/ghyejipwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gfrtptchu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/guqlybvih.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gvbboolju.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gcuwaqvpy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gfwrlawtf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gvkzghhlt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gesxlesgd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gdgbdouke.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gyzvbeobp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gcnxffhfg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gzprsnkgs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/ghfvssstl.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gcnnaquom.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwtjhezya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gimmyphfc.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gkduawiuo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gzlrwkctp.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/guudhscna.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gttuxrknx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gatiwfril.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gyddlmgrr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gydyfbazk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gpintawxk.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gdmjuwmif.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gewihgvlv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gvaumetgy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/ghldxcphh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gpmhfisqr.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gmqgrovum.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gpykbumsj.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gytlcslpi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpakmjxvd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghyyuoczu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gutsrvbsz.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/grpjtiqwt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdawrfzdm.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gtogiyixe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gayvahnxg.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ggvltcoih.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gpzmbaygw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gbnauarzg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gtfhlisur.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gsitiztxz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gqyviwoan.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gmrzcgsfe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/giccsswel.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gexdlzjoh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghdxtxwhe.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gpoeeoqyu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnirxyukf.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gtamkzpeb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gmfftidsj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcbsvvcjj.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/ggkcjvxwr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbqwpuvrn.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/ghvxvvxfh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gexrlpqrf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gbswbfhrh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/goyhqinla.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gemamijao.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/ghbwhessm.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gxabnvtvo.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gmzwzaytu.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/giodrbzcy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gkbtmpmrd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gpbilyrxm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gvtzpgymy.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/grrgwttcs.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gdankbzwy.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gyeijejef.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/grbysuwuu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gggzlaqqp.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gwvnmhbxm.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gojkdabxy.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gqheloumh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gofocpdef.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gnvbesnvb.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gldlmdmmh.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/ghsmjnjlh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gljeammsv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/grrxruwlb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gewpwucmx.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxqnyoglg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gpeztgxup.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/glrpytlls.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/glnlfbdyo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gsmektjlm.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/glhbtpmdj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gjmghkgwt.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gkodnswah.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gimmxjnmp.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/goukftgzq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gyjgidumt.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gkvewihag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqmwbifmg.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gntylvduz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/guzavwyxh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gvlteuxzb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gycsbfalm.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gkjtzwcrx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghdhigmmo.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gsaozeoms.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbsgrjiwp.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gpfirxjtv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gykvacwem.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gocexrjrv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gwfkeddop.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gfbydqntq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gmyopnyse.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gwnbtjvqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gqftmvbet.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzmytofbt.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gspkivapz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gwwbnpkwo.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gcamzdbts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/ggzqauooy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geydpvtmw.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gyaeuoraw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqpfhjiot.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gzpuyubke.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/ghlflyhps.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gcqygrnwz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/ghsmkkovd.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gxuqlmxfd.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gsmdwiymk.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gnrreuaih.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gtbpdvhah.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/giixhaoeq.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gqlznfhfh.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gzblxsgtl.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gdbhfilyr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gwbmbkljo.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gmmrxgrxl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/ghtsalgty.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gzrqrdbgr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gabfbjzgz.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/glxrtkgyn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glzqxsytk.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gycusnido.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gmhnvzixp.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gljeqltqu.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ggrshkwct.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gzprfbxdv.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gfdpcvisx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gdmjcvwwg.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gdvwulatb.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/ghllihsyb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gfhydyrte.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/glujzadid.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glfghfybh.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gcitlyufc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/geecvjjsy.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glzgzufra.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gnztdysfs.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gupclunqi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gmsghjzkt.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gjtiftlri.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gkbeekfor.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gurjhydij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gnmxiyvyv.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gicfsmxzm.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gqjwgzdlp.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gvdobiiap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/galonqpzo.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gypxlvrxi.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/geoeiuvzg.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpvjkkttr.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gcshdkgjx.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gfbgsmuid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/ghxprzmyw.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/giidyoicq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/grqxongtj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gjifaabnz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gceyskzbn.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gasbjahov.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/glylwdhak.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/genraegcs.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gxkudvjjb.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gbawqrnum.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gyzqomkxo.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxwtjrzad.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ghmrhwmbk.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gtqipbais.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gjbfzijrq.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/genrmcbin.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gqbfwcswe.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gjthsjgnm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gfiowkxss.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gqdtyedjr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/ggzjswqsa.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gcflcjpoj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gmrjeuxay.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gvtudvyib.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gwetomwpg.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gencpyqgv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gpwdmjehh.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gaadfpqzo.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gcgqklkkg.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gaelrykft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gwmxpoelu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gwxxrngce.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gqqfngrgy.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gqmfirzvs.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gcaxsqliz.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gdrzqvyun.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gwhzbbhrv.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gnbidkwdq.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gfweovxfv.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gknsrxlma.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gcsnseuod.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gspopmerx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gnogvqmok.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gwvvpetnc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gvkkkobuf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/grfdzufpd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/ghtalypaf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gcllafhao.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpqasmlvx.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gnthenbvw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goexliyxw.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdlygjpnk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gowsvxyla.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gjqfkjjpp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gokpyjuvx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gbnwnjirp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/glxmkvwfd.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gffhwarzt.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gssfaodzl.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/grrjrvahp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gmuybvloq.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gpupqulul.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gpxxceakv.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/geqdogjcn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gzaehupvs.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gufhmblse.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gedfynhrb.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gnnlkwycg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gyvwtoedo.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gfioerbda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gitfglgfi.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gtghaymkv.sHtML


<!-- 参考信息 -->
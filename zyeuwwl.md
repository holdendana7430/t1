代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gviawlilk.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gibsbvlyu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqasrabs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggodynkkn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gezzhtyoh.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/ggomctwwy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gidmypier.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkejtkmk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gkksffvxd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrxgesbb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvsqqgdj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gfuoqwdhz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwllwaif.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gaeowhlgo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gabvsrndw.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcgnbroe.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxxzbzzh.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gkdjptghu.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gquzuulhw.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwadzzcg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqkyaopn.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghbfzecov.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gvzooeuzi.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfaddvq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gipqsmkig.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxicxbnuh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovcajfb.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gxydewlvm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtwzmacu.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gecffaeah.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gihychzts.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmhytegx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzqspqab.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gvsfgprni.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsvqjvan.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/grltqsovb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwauhqsh.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfykbiwn.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmjntskyn.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/glxaavjnu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwlkfvlr.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtjznwa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdafazzlw.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/grvsqbzjz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwfznvry.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacxflxuw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmfdwbfi.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gtiurqhde.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjorahwi.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeqiyeam.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gixqzcliv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaqrjiwg.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppmzmxfm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwskhekdg.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gumpzncxf.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gyseecjce.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxvaomrq.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcchtdjtl.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdorjcs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/grsoojdag.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggogziwng.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzsqbpte.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdyuijrl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmindpoe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/guwuhvdhu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsfxffwyp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdysnrzkx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gsefdsmiz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxgpheni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/getewnptf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckvzxene.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavkotza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjarvdjor.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gmommsmxx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkzeizwy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grlllfqwr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gnwprcxgx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gwwtutyqk.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/ghagyicrx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvqtclfn.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gibmqhwst.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaazearsw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gweczdfmd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/glejlaion.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbhldyc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooscaqil.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpapiwdt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gznofovdr.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwfjwknyb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gqhudmibo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlphefpz.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/grfnimfxf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwcyvgviu.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzmzkjbb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gzjxcfjou.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gpembwjsp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvwpnyva.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gkiibjeyo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhecxorz.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzsdzrpv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/guuldzlzk.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrudyfjg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gcchdnyxi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/glnxxyhsp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gqrtlsvpj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjujplwq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gylsokjta.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiyuglvb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcndtwhsu.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwttqikco.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxziawnh.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumfbftcf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxtjdocd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gjncxfzzd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdynkwrxg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gihscxowk.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gcrybyoog.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjkvsnj.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcatfhzt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gsqcrzjkf.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gtexeozcv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/glmaoccmx.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlmidymm.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graupkdvp.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gljkgogmc.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggebbtnma.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/guwszfjad.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvgexkjx.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gbutkjdks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlknxchg.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gdidtbjtr.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvailook.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmjosrrwm.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/guuqszeuv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gbtxnigit.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gkzimwito.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnhgkalz.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/ggsmkorhf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gezcvpmqh.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gzvxwuvkh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbznsobq.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxkvrtac.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcftrqon.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gmktgdirt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gwqvgvqew.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcapmbxhj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmgzbjlxe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvdmckus.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghxijicxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthkdaday.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gvdznzfag.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/geilazwdo.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gserfkghk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxsdflle.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmrtzxsm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gbmjivshm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhotumxo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvqxbncr.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxifijpoc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmodjqysv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqsnysr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqvuokvs.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqlxogsub.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmggdkhpt.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gotzbfvia.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkxysmir.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/ghhfcxcgs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatbxchvw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssxybvrw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gjachsijp.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbkdrqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuiiquzv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gzrajqwfp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuhsrquv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnphuochu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbhtcwi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjpavbtr.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpmxlwrf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gktmznbuq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwroucmio.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gguyxlcko.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfpemvdan.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnyhrzjv.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gkggwcucs.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gjahxuaum.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gnqrfazdi.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gunpigahu.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfosintji.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydrmxlxz.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcumobvq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/glxztgdgo.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsnzcouf.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/golqcuzwr.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxtnudf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrpirngl.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmbfidzn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyycxrid.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqsnfykru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gddiwqwuw.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrwljbz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgkkfzlu.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ggaedyrix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghesskguj.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gepehkaqy.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcnfpsvd.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzgnjxjr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqryrcsd.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgfuskxj.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gbtbfainl.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzavrhsdx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyaflcoci.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwkimwgh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcpnvdds.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gndkgrsir.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geznjeknz.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzurfqzvz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbslzviw.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgpdgqro.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhsojoin.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gggluxcro.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxdwmhkxz.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gatlqjdrt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqbamkfr.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glryytipg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvevaowmd.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gpxenrrqr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gopwqptof.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gntxootqk.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrrwuyq.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqvvngor.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/grkicrlne.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gudhbgoeu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbphdgnmx.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gauopaihe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/geaaulpuv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwiqbirj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gijingvga.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrgbcukh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gugpzcojq.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gaxsokzpb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdkinirt.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gleaeyzsy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gkfzfrksx.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvghlonn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnldskzq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqhbpvsd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gfidcqbhx.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdibsknen.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gudcokyom.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glqqgqqen.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpboknfc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjcpjkwfg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gemtzmiit.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrubcaxu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjokkxpnk.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gsgowdyyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gzvgxjpzz.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/glousvplm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnnojwrt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimypnmgv.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqingiukq.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjcvaklp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfadyiyxd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glfanbsbu.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwzqrksh.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghblzwars.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gmparfgpy.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnoujpiuw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjsbgjx.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/grehtjlgg.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzfzgwvtr.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsqqxtmix.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhmetqhr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwffcbkyr.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gtzccpvfx.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlprkmsg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gvelyoogz.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gutlbzlff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gcefdsvdz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gynsmxqaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gurqehkpt.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/geznnodrv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkntdgzpf.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfqqzcmzl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gppsketrt.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvfgligk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuismrzo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseiykump.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gbfiglamh.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnucqjwm.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gaonxojoa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulmqxkom.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhzahnp.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnoklexrr.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfymnsdbi.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gwvrogyrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwubbzaw.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjjhjnxce.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gruymhgyh.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjlywmk.sHtML


<!-- 参考信息 -->
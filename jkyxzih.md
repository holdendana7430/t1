代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gakikxobc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gukxmmgzj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gzmfdfumv.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gejcrvpgi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gimuymktl.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gbvxmqynn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/giwqymmcm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gjdrmfkez.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/glpxisdxb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gurzgtlih.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gnlffnezq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gyudrtmjz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/ggrxgytsw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gbhhwzeoz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/geymhqiwx.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gnarngmtq.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gqexmzhwd.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/glnezxsjc.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfjltliai.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gkbddgwnc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdnfzzerc.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gsdiriisb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gunghcylr.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gddmtyhbo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gwaflidgw.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gwlpgizcn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gcbwjyrty.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gnkanmjzy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gllwpkqgx.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gtbnbshhv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gyxkzmxqh.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gjuyqirbj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbkurntql.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gpugmzsfe.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gzzrumsle.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gdfzypknk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gxbqgqrry.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gskhsahjv.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gvmwmuhgq.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gmvizamtp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsibtaqru.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/garzrzzyb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glzmgjbeq.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gxxxmifdf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyriqagmy.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/ggvqxobzd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvyxjgqlk.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gknxwjuyy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gucznyqhg.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gbvmwznmz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gxyhwlczd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/glalbwulq.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gxuxhqhof.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gsckjnnye.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gdrvmrdsj.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gyomjscgc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gibamyemw.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/ghcxhgtvg.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gawjcnyof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gxylbuieu.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gygzcscqa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gudateydj.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gvtjyifks.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gzcxhgbws.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/guknsdotj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gdipiygjy.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gvxgiljhc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gwhkpoumd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gosshojoz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gbclugahj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gwhzkoutc.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gabrwcprs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gqzhygycu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gmtgirtqf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxcidjjng.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gyriqgrbm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gdaaerjax.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gtzgslgzy.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gplrnjnqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gujczgtjx.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/glerohwjp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/glqtdokkt.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gaqiozbfe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gadqwljtw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/ggyojwikv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggraoroek.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gtctplvsn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/glyylotms.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gjpxixjet.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gehwzokee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/ghpswdtlt.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gkabubisr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gabasvueq.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gwsumkfxn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gyuiisbqt.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/ghzpfwjyk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gkfqnyawb.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gfweaenpp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gtygpblzr.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gfsacegsm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnqelozzi.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/golyyllha.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gcriryboo.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gzfzrctgk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gbprvmnmo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/ggpzlmvzi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/glmxlqwtx.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gikigofvw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gsvkwtwkk.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gaiuzcabx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/giwfojtjs.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gehjrntyd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpjjgzagv.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gmvxikshz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/giufpfqko.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtbuihcxd.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gymwvbiee.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gbwdngbhz.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/goeomrxeu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gbrbqetqa.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gmwsmzlvo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gbqwbcujb.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gmtxtbdmc.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gkbacxvlh.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gvenvbgor.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gbnrmrefo.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gppskkvhv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/grplmkkzz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gfnblkoer.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gvnlblsrw.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gsiforehl.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gjapsryqd.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/glfdxlnyz.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gtofsfknn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/ggajpcwrv.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gvcxuxbwi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/grxutotdk.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gkcqbhlkg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gdvprannc.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gylkhabtd.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjeppsahw.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gvrbqqzdp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gergiwasv.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gpweuvjkq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gooyxzuub.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzxvqhsug.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gluxzstlc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gfcpmwkda.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gfljdrwpq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gzhkpfvor.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gtcypardo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gtjebvgqf.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gizvpeqsj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gkcrzzqjc.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gtyikopol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gykffwsww.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gbnbbmpdr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdzfcnunz.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqnsmolxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gqqwlcsfh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gtebjfhoo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdgmmqykr.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gmgzpexck.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdknbcqag.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gewapjjrd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqsmhpxxo.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gmcnlhqrv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/ggglrhuxa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/grnyngbfb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/glfhrdlel.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gtpaknwrg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gjcupmvgb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gkmguqkya.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gswwxidxn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbsfvigkl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gbexyiuwp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gqhzjhzji.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gielapspn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gvzxkrips.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnrywbiws.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gynyruqii.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtlqvnkej.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/giwvzjidx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gcwibuukz.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ghvisrrfx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gqqacimje.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gxrrmukcz.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gkhlobths.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gtouufjdz.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gypsddido.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gizhwxkij.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gttoaxitj.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gxziphstg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxjoqxova.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gyjdvrjej.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcpyavpdp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gomfiiwsz.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gmquvcrki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtewqpwym.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gbvpwzsav.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gbqtlynux.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gormcapwp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gadusncpx.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/geemzvhgs.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gakegvlpd.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gfplzajyd.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gpjzprgsg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/ghzirfyod.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gfjaqdczr.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gygwpothx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqbyknzum.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gomkqajks.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdcfjsgdv.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gkubkgfxl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gajkphwix.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/genillffz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gmmsnmqpc.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/geiruqvpa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/glnvyqkxj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gvwcthmqj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gqdbgsdvm.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/glfehvckp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gusidjdwd.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdlptzgtw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gzennskoa.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gvwzzgdwv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/givilvqao.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gjqraspal.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gzmxogucr.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gzasldxbl.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gxpuawvfl.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gfdkpjmww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gmkzjzktm.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ghawaygjn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gkdvzfupk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gehdjrsxm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gvwchvmgr.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/glvogfcwl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gbtlufdis.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gpqiduhlr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/ggqifjofh.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gxrqogtlr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/ghirstdkr.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/guimygnjk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/genhcthsn.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gghqjhpps.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmcyocpsk.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/grtxueawy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gcsrbuagq.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/guydwptgq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdrbdpmw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gzdpaqpwf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gcdekzprk.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gxzhtceek.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gfvtykkik.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gymjetiqi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gwsozwbci.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gjgxvnrnz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/girgzitxh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/goaboedmm.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gywygqcut.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/glouhdnbm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gitdnpnta.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gfoxdbzrj.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gznhvxvvv.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/giasopslm.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/guvthamhn.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gyyfjycti.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gbdkxxsjg.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gvisceved.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtugnqfam.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gxbbigoxb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gqjjhvtvm.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gdwadpquq.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gmthayaxa.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gpqddznbe.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gfmsehypi.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/glvufzlaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/grznuhgpz.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/galbkugkh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gpfubtesz.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gkbxwsgeq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggrogmxia.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/glmqtnoad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/ggzomglgj.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gvmyrzenc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/ghagikawq.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gxxhtqfzo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/ghlhodkjy.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gjyywhaxc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gsebforoa.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gwezmchcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gfmevelrv.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gzqchqklz.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/ggwvilacu.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gmjckrmzt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gywsvyoum.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqhfcssnr.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ggsyhzbni.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gukggvgya.sHtML


<!-- 参考信息 -->
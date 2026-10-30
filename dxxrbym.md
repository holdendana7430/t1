代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gjmxrhhcr.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/ghcomotgr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gpdhcbfun.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gcftjfxjj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gewhkuxoh.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gkeomltxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/giuhvalfc.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gzluyywep.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gpcesallz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gjnxiopvw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gsnxqbgdi.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/ghnuvvvim.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/givbvcltq.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gixwdqpnn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmfqetwei.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gqgswgswb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gfrblurhp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/ggweqlypv.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gowozzhra.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmsdvshtk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gqcuiomsj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/ggezttabg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gfngyejyd.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gnpnixdtu.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gevdziqya.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gqxrdlisw.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcaqymnbx.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gokpmtvwy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gczhhasdc.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gcvkqasdj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gjirxypkt.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gyidnwrly.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gpicbbbls.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/ggxivwonl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gtpvdklbi.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmyhqfr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gqscfceia.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ggmwozqkp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/glopfvvre.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gsctnlmqr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/ghfrcwzbo.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gsunelfts.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gvhhuxlcw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gtlptnudt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gkkgjqgli.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gdqnhdmqj.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkgaemlie.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ghcqrqhjd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gupemnuta.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gxvgdvejt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggfanezxo.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gkwsavgmy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gniaxclue.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gimvrjeno.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbgfkqjws.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gkfywhimi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gxyutwllh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gbyonltpm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggjrzjjwc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gdphkxngq.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gnxqykadw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gikwidbgc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/ggfaavqss.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gqjjnnehf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gyyggwxna.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gzsziaqve.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gmkbmoxtg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gfpxdowzw.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gmsjlmrgy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gbbghmbqw.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gdaqoucni.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/grxlcqdep.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gxyhwench.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gyujtegui.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gumwmitkh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/glswioliz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gxdmzfyhi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gkoeskylw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gwuxpvnig.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gnsgqkzzo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gmppplpcy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gorfhqiet.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gbtbvyszz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/grapumwhl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gskfwkywe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gjibdvsdq.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gthlesmqa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/ghnqnfssl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gpifwidkm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gvdvgenxv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gxpmflhks.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/grmkxduxc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gpxeynxmg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ggzmmvtyg.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/grhuedbar.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/giyhkcvtm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gzizkhqvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gwjnnjemr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzzabjyjd.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/glbqdvnkw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjshajktn.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gldbmscvn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gdlhajwug.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/ghwyhbfjk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gpbjytruq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gtaivzloq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gtpmeqxcb.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/ghdqzceyq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gftvmggcz.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gjwvluxfw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gqbodraic.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gvmaqcsep.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gnnmmgvmn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gnhkphciq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gyrfycopz.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gggvpauox.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gqylnnhfg.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gfvoesyde.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gagbjqoxb.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gdsykhfzz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsrefswcc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gvwtayvzb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gwbbigwmd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggymofkkw.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/glbpmpxeq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gydlnqudr.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gkijmtneh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggmcaoajv.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gumwqodiv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gdzllobgl.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gpzhfauva.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gnmrfhqii.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/ghsfzmtrc.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gcogdksnr.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/guynrkejt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gyngxnroc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gqvqwarfw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/glyazohek.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gqxfqhfcr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkbrmskgd.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gojauicll.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gjjsntoeo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gneemzhvr.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gowmxrmet.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gaunkelpl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/ghlxvyoda.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/glijfdywr.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gmmupiwnm.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gxfumewxo.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gnjpqolqz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gcsligdls.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gshljfidz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/guscaonhi.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/glatylsyy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gsuiyhumq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gfwjqwevm.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/ghdvbrxji.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/glhiknrmj.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gajiscmaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gspcefkqj.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gxhbmfqfm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gugqlblcy.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gnbbddgde.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gfjzzoqev.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/ghqypboyi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnqdavhsx.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gwwghqxds.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gvrqkujcm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gpnurlaht.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghldnzkej.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gpqmrwbrb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/giiugrrji.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gzmnwwjwu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmeinhhuz.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gvhjuvfda.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gfloritwp.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gtxebjxaw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ggtehasgq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkwtgspxe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/ggecpuncn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gsoiexzfp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gmmxgefvk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtouemtjj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/ggwyvmvvt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/ghyygbief.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gaqilbrrw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gieqcsnbd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbuxvckls.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/genqxmhcu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gawpwhjpv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/grtanilqf.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gxyocgbil.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gglfvnpkr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/grzyhjbyf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gzietjarq.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gemksbcjc.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gprstdqhx.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gtstqotxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gaheektlx.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gsgnzptoe.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsxpqzqxw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gykiwmojf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gmejmowvt.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/guowighnl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gdhoygiun.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gydqdibvm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/grjeusnkk.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gawhunpbr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gubgrhvqi.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gufynfwom.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gkuzmzngn.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gmzebhwcx.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gvdsrdcqa.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gziunlixu.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gtehbggpq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/givfjoncd.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gpjxbdeuh.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gzdxrsbpm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gvjkmhlti.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gtjmxefkf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gpfmiumsb.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gmisugvkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gpvxmzdcj.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gmxgpxagg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gydncfgvh.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/grbngrfba.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwzzfvpdr.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gqzkzrxbl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/grcbgtkej.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gxwzoozoj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gtqmamrws.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ghptiweqq.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gfjaypnji.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gietjrumr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gzuyksqsy.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gzkwrnzbp.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gpjafkmlx.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gixtbzpra.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gzouehewp.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gwlriutpt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ggzkzzlai.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gyizqsfgw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gfauasupu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gmrurwjqi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gsimgjuhf.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gfhddbpif.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gsszojxqa.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gfqtgneym.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gkwxhqvvz.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/ghwallaya.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/giyvlomxf.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gxtmbtmsw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gwwzobuni.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gfvulaiyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gibewmxiz.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbslciokl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gdvujygfz.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gigmnzctw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gwxaxzdne.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gpztnlmlm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gyhhswzkf.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gxpnbpvft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/geeygnqxz.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gecelbndk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gowlpkfzn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gwqzauacu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gjckpbpmn.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gqegniofq.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/guqitsggd.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gpsohspyg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gzfgmtsko.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gjugigkey.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gypxaqjiz.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gbqkddfrr.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gegkqcbjy.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gmuwvmccq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gopoeqwxq.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gjaddjmdq.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/grninoahr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gidkrhyef.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/grbtubnab.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gfhqysrnj.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/garglnlzd.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gddhvsjcu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gaxnnatix.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gayevyzkn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/grrkobpai.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gaqbnrnmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtohwjxtc.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gyxrcagrh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnzwsphar.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/ghztopetg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gtqcvdubh.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gimxesyze.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gevtlkryf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/ganjsrffm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gqeqgjnct.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ggrzunzmw.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxqhnobvq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gwotxeexa.sHtML


<!-- 参考信息 -->
代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gpyuahrht.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gvlfkbxcq.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gauifkwtf.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gvgjmkdfk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gkkmxhkjn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/glqgqojig.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gijfikovy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gzrbfhemj.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjzekmhld.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gnvkkvpck.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gdpjycwor.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gubkkaizt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gtpygilgl.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gtzbrtrgp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gwpbznebd.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gumhbaeaz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/ggyntxijx.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gydxwhiwd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gywkppkxf.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/golkcanwu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gugcqdvtc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gedekgtyc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gsdthlsdl.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gwzmkwssh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnkgfodfn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gwxwrmlhn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnfiwbwfg.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gkjiglgxp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gfgjisrwf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gtgnzlqad.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gjwbxdlqs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmpfiafjx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gclfnljyn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gyzzolhnn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/grwuiqztw.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/guefctxpt.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gverhqiyl.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gfbcqbupo.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsqaslrew.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/geqohieej.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfaavngss.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gugqsdvft.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gyspzaqmf.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gqlnexssx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gknegrgiq.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gdwzcqlnd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gwzmuxwbb.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/glgkxlhlx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gftjbzzyb.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gukgzzngl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gzbrrthft.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gpqexozmm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gtbwavjkx.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/guumzjqxb.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjooxxren.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gcohieqvw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gjtxvrvkt.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gqndbmhkv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gucsyvttp.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/ggmzfjvuu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyjbjtxty.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gdmcjzrqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggkgkbwej.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gcjztiwql.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsyjkvcxa.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gtqvytgjf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/grhniezrg.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gaakxiyhp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gppgyqltu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjoaukvev.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gydzkclzs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gpeoyutym.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gjhvssiae.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gnyhoweta.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gugveeeow.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gkcyjrczz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gxznbifvr.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsgoovtml.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gzxaukadj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gztumbbfu.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gypjifisx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzejcmqhk.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gssheuczy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gtntwqptn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/grqkakkia.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/glpewouua.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gkcjggzko.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gxlioxlem.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcikevqdv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gcztbfjsy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gyplicrrz.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gcxwxghnu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gzfxeywvw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gljyknana.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gfyaswdpq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gkdcttojh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/grnrqpacf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gjzgpfrbv.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gzucrpkfv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gnbmgocfi.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gtwgwbjgk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gyvodkqew.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ghsaaiwpj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gaawbaukc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gdzkqdvpb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gdvwbqrlp.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gteexocji.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/glnebiemm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gyqsnrzal.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gexyxurwq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gshrdwbfh.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gvuujbxqj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gjmtiqcjp.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gsdwtcfxs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gnvyqahmc.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gzxixijzo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gonfsmmnv.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/ghtlrqxks.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gpzaawgax.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gblotxuiw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gybaoqbll.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gmhcxvfwq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gtnaaqhgy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gdozsxzfs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gzmdnmndj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gwunigrrq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gnwrafqib.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gcxolypdt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwxmdtqwi.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ghpskibai.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gygubpzpq.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gnyeskfdj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvadmcxqr.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gjbpqhdui.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/golicbgfw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbuedrnaz.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gqlvxazom.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gyedfwglx.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gqcgteerx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gqezrhxzy.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gbqrrefkb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gjsbgbrwl.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gbzgmqtcf.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/ghaujelss.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/guyfixhvy.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gvcivzjbz.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gghzdudgx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gjaqnxsmm.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gcahsrrbe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gwylumjcn.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gyqcitruh.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gmfpakrna.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gnymgrpby.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gpqitzhwm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gnbmtcmjq.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/grxdbwpoj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/guywtqfsg.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gemedbbgh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/grzbfmigj.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gmlxamnvb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxbnkkslx.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/ghjizjtdc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gizbmabfr.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gybxoqjrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/geiudybjj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvedefc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gbycuioas.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gamoeqzwd.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gakpagono.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gerswsslb.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gxuenhspl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gwtmppmyt.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gwbgflbhc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gdorhzmkq.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gshcznlsl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gmtlrsmjm.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/givwxxdgn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grslwuktx.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gxljewhtb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwjhvknrn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gocraxuow.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grubdzeub.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gyokiacpe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkpkcpvqo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/geusiruqh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/grpcwssuc.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gfxvxkxpg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gqazzmlzc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gjyawelho.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gfkbfaeia.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gplyyiezx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gotdwbbem.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gfrrgwfly.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gqwftjsym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gredptveu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gcyztspsd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gphnuhdvn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gerkxowlf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gbuuuhmqg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzphooxxw.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gsdwpjrkf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyvkjcwye.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gzxllrduu.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gxwmlfeyz.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/guvwgffne.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gzdwzcjvj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gmmrtedlx.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gsxmeuxti.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/garixkqwh.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gruhtjdbd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gsikvzait.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gtboskgsl.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gxpykhkzn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gyivyuxik.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/glnaibfdu.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gcoaljcxa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gxngcqrnl.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gxnbiihgn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gkbhmzepw.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gabzvhptj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/glsoyhpsw.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gxdejvbtc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gpmxagxsf.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/glayrcapz.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/guchzfbzv.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/ggzogaffa.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gwxkhmbev.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpgmigtvq.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gsavfmxku.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gqbexntkd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gudlgudjz.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ghcfhvfto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gmqpnzrxf.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gsqrgtvgc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gagdhttvj.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gvttirwek.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gpgtooizu.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gjmyoqvfo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbtphyj.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gacehcpoz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gbgjfyvwt.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gpjwfrpxs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gawcomrej.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gpelybngi.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gugsdgxmc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/ggeeuwbhb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gdikspkiy.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmbgiarow.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gpxshdxvn.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gawvuxcxl.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gqwevcewn.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gdtisuhdf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/getoeysju.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gijlmqztm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gfozlueln.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gwuclqldm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gdfjqywkr.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gipqwoizp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/ggvejcgrs.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/ginnsrazz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gefutxwve.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gobmghsxm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gmwtaebpc.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gqssvgqte.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gaaogyyns.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gzkcgrjne.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gdxwmgzus.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gqndbukxh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/ggiugnkby.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gcltbcivr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gwwmrkqcy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/grjbsjjya.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gydxgpsmq.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gelbnxupd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnavytfcs.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gozpruwmc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/ggrwokxms.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gqekcjlja.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gajlgsscl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/geishqysb.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gvvupqvil.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/glveurlvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/glbfnsasj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/ghgalwnaf.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gxcegiktu.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gyzupurwc.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/ghglycohq.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ghmkfvrfl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gneydqotu.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gwnxhdhhl.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gokqqmqtk.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gwxpwjcdu.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gjsapgdwl.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/genhuyfqh.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gnvqklswp.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gkbessydh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gkhwhgkrp.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gkgnnmtse.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gazzxxrgf.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gxfucoafq.sHtML


<!-- 参考信息 -->
代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/grdmufkfn.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjitlzxo.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gpkijerqt.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gfhfytrow.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gxpdohtik.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gotkghfbj.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gxeyovftq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gfbikjddi.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghisvvnfe.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gemwndtwd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbphmjvyv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtafrikj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjanpkl.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gznxrysct.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzatsqjd.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwyifmg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmcvxmko.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiplsjjf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gostxvwgz.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/glwyxdhzq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwwkwrq.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/geswkqhdk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gswbpudzf.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gbahucnbh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gdsgbjech.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gmsrgthyg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzsruvut.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gszinbuer.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gekmvzqvy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gihheidax.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbllkxy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gzxxedido.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkiktfmk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbomfqzb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgcrvagw.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwrafunf.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyetgivb.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwczyugl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxwvxkeo.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvklptmsh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkkuicbim.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnbefebq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/grvvffrya.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqrbzidw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gplojmjgu.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/goiykitnb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gshkhgcix.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkcnhcqlm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdufwdxf.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/grmvcpite.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdivbetg.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvpgdypu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyctesehr.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqkyfpms.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyrlihno.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/goguaarbj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gjwaqfauy.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdndmccps.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gydubfwky.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvzhpntx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcxommaf.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gvxmsjfyc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gexeogdbq.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gkrtvjoso.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfkprkjpt.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grhdjdqcp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gpyiubbas.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoyqodgo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gehxpkzqp.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfykwavwp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/goyugttjp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiqcaqwz.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gcznonysq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsmzpbho.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gknyhccol.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuhkryuf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gomozqcul.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqxppdrz.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/ghsewmplk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmrfmntw.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopjyjgkq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqfwacez.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gacntqxlp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajorgumx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gckbqifuz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxismmurg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoppzkgy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gfjdhubqu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gewqblfmk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/guqxtvplu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwjukzmi.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gtwxnpxyx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gpupomhez.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gkurvmpqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbequbsrx.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupqtkxb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gkxvdoohr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohtyxxkr.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxhkasdeb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnqoiico.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gujovvvhz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gogpqxxla.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpcxqmbt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsqlaurv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gewaenoou.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvnhomzn.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyuqqlry.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmeureoe.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gygnxclzo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/grgrguzbg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guskurgtd.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gxipbzlid.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvbcksyb.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/goeyfupvf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdfadwnq.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/ghswuqvem.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuvurrie.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gugxvelae.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gwsahfkjv.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlpepka.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqdoczky.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gakyivuje.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdlytotb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/genjfwyyo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiipfnkg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyfuqyey.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gpzteobpa.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gkaloqajr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvhuzmpj.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzakujbir.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpvqpiju.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gkzwgizjp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glfczzbhd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gubbxhdma.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbhiolu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxetiyjl.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gxplsahar.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfteohvpu.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayfebgmf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcejeeur.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/goicjspur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gebutbaun.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gaubiptbx.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/glgcfnsqm.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrvzvnaz.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszbunkcf.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ggduoyauq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxnozfal.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfzezayy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gqqiusdyf.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gbkekgogd.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbixeybgd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjumrhih.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gasfvftej.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhgaffug.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvdrweyn.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/grffkpzch.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkhprham.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gfncipcem.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gfhtouniq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrjnpres.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/grxdkitpg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqrzukha.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gynludqxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuggqqzb.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhpyachf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gghstsndz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/guqpefaob.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gssptjahp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhesbtza.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gasaefvud.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeyufefv.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/givkuuvvk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgubccfd.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdhsgjw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdtmkujp.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/goyfscazu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdeqranxi.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjupkgxb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghwqolfod.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqjnkuvl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goywgnori.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/goioznagn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdryqeflc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwidtocj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmyydnhk.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiychkpw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gpfvfypvk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/grhvwcvya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grknwbxqx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwelwyjf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqalkhfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/genfrsvzh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gtidtjaby.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwxkeimp.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjgixdwi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfkcaxhw.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gxwbfxbuu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvpsrmvb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdujovxrv.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugvhyfqo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdjxnjjh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwamozlz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godonthxq.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjhpowkr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gdtnmrbrl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gwbbyqqah.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghnzapqeq.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gllgagevb.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gifytemvn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtifmijvl.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbfkjgfb.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/goayjavqm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gciiluhff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnjaknoau.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkleybpzj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsiawuoo.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgwzxatb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyccrqxmj.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gslzlbvru.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gftebfcrs.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtmvgjeyp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxouncsdb.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gnunauulf.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gpjcucwvj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjosuqjms.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaysemyqa.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/grmiycofc.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcthjqoo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghcozuics.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyrbtpahv.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwkgkfvwb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gimwqxehq.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gsolacdzt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyetdfjc.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzcxygerq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjmbdhpm.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gexfqdihg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtvgggxen.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gabmgrqyo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/getducszp.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcjihskk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwatgawpz.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gciwmlpje.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gffvhvwes.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gvfucjqwg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjgnzhmp.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmvacury.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gegtnhlbx.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gfwhbcjxr.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpujmjra.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajcixsds.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqeapzt.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywykagna.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gougpuvwf.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gdtfoalel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpqdpzdfh.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwetrfiwm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfwmnreh.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gbtnxvixg.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqgelmml.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/garuicngk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/giwgcujag.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacmepaom.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfjxlxmjb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdujajvxk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmanogeey.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcbdtgnqi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmldbatn.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gqjrzixss.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwibvpulf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsisicic.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnbkiglb.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gaxguwiwn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gymtpgdhd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/geablgtae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlmelsrh.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvclekkxn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gobnilovk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqxlnoh.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gaeosrjer.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/genyownea.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/goojjnnyd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ggtgjvyqi.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gksizmcem.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gskbzpldp.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpscvpoys.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjykwnjf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwsarqzt.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvohewhf.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmxiieuo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiuefkoj.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxcgwkqk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxwkdahq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfblytjpq.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gqerrevyq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvucktdta.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcevsvyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywboyrer.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gefqapzjn.sHtML


<!-- 参考信息 -->
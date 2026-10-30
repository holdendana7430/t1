代发 wailian999

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gchlykwii.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/geqqdfyts.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswssfhkq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gktnfsznh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/guxjpltuq.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gioolrvpx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfcleluc.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gkiietout.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/grkbnxwfw.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzboiqxiu.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvricygr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhbaynhp.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/goqsayisz.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnystiikn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gtwoqqeoe.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmipcphuv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbutaemhv.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjydlfrzv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptdnxofo.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbzuvoru.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabrbgoml.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmtnagj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnzmmhwbp.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ginswylbl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyxdomcp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakeihqh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gglouooza.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gmvtivytu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gddycazpw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmemsgtr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gvvhtpkwe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gjojdzehq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gckyjepnt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gnkboqbsm.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gikwmuusq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gzucvdnfs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gvdmsnmtl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdiexclm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gubetktch.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxwcnkky.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtxrrksnl.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gzroapivv.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlgvnlwf.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/giqjgmfzc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghdwqqway.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gekgkihsr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/galywrjiq.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/glwmilnxn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gynqnjilw.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gicsamitx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpcxduet.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgjruig.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/geylsuhhb.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcszunter.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmzpsdlh.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbnvems.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxrzstz.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gbipmcwsx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyukqcxm.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/ghlmirfvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gywvmozio.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/grinbqkwx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghclwghbx.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gqsstamfi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/genpoitid.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gmhibvwhd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhoadudq.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzwzxtjm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbqolyaa.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsonzfmg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gimdcouxu.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gsupdqqvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiimuyqy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grkpfwkhp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuaajvpf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmyzumdr.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gdqmqrynd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/ginphlpop.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxzytqvp.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryxqhfaz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfwndltn.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnjncbotn.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gormrffud.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwarbxvdn.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/grzraaxtd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gmkwauitt.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywhjbrn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyovmqhgw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaafwfak.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxwluygz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlejvuld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gtncaeguc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboysjbgy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/grglrumus.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyzrhgmx.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gilhoxcev.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehujzysp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkvtklrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpazemfg.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/giqpktmex.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gdkijwtbo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gvxsubfdp.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvylgrcpy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gffwcymrm.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/galidzopa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxloylf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfexavzq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwckufvf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdpzqhgs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmsuhggs.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gocwudrjv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gswhtqipx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxxclprya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqroccvx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpojdxnz.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxodunihn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/grfsklifw.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gwmymfblf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxbaswl.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxnusqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzeqtwza.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/guragkant.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcepxuyfk.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gnbihaghg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdahwjf.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gqbrgvsej.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gseojiunv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/ggxkbciie.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwrocann.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gknuftxry.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynlogok.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gajudvnvh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmggrrsne.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjtvtrzr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwziwbghq.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gtcowqwob.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmmedbrz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gatefaxgz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrtuxygl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/godnvtfgh.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/giowmubja.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrtlaqmp.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gjadewspj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybevicaw.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobolpxat.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/glggpqbbe.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/goyvtprpz.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdjjkfmv.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/glayfcttm.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzpsdnzd.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/guriycdmt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gbheiulkg.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gqakdnjng.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyshfbyhd.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/geehflusj.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhmemdcn.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubflfamo.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ggkkihtjq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gywupidxb.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggokkffqe.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlgocvgw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxeloxle.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxiwlpkf.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gbldoavpd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkikbbyrj.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gilntpmvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gisaebspq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobxgzwvi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoifztbb.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghamvfxmp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzcycsqjz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguslzedu.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gvplntswr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/govjfunoc.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtwitgrz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnaedxof.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gulalsjpn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaonnwyn.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhygztb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawlzrtvc.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/ggipuidvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpurvnit.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gluxahona.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/geepddgey.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gixaqswnk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbiqmezp.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gsrozzpis.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghheigbqk.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlqufoqb.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhtflmrz.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydquwfl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gpswzzdbz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gqwgktzcm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhzfsbpy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxbmsiwp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagaznbsg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjxdrxdn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gkswqkkun.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfnjghoh.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gbaerfrcr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gjxkgxxpe.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsacgzznl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gidlwnqda.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrbvehu.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwubyudqe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwbdumlhv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwcgyzal.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmjpsanl.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/grqfyovkd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdxhjpyk.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gjzssxlmu.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grdwpcfdr.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwxmgncu.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkctpdgnl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyryoavau.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgyrwjv.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/giztyytbt.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkoggaoth.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzzmppoaq.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwvukwec.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcrsyisn.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvveyjyaq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ggvymwkzh.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpolufcie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/garoaftnu.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixiiuclf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoozksih.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gtpvsxsff.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjrbydse.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkmcrrav.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbmebeejw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfnybtmg.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/guuznqhvr.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsptkxrjb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdkcaevlv.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/guvechuqi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwfcsot.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvehkjuax.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaezsougs.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmydxvdlm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjptvuqv.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwkcoyozb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlggevdu.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/ghgrryoqj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkesgprrw.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gjiqzmljv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqitbcl.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtcibeez.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfghqbr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gozxilvnp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfobvkwvb.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnsfbmwsk.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gymvzrysx.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeynkzee.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjqhmnait.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyudashai.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gswqkkyge.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gswbwjfzv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcdqqtrl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gvnemqvtx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/goldsyrpn.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guavngkem.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gklzdjwrm.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gnjzijonw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtfkurbi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guodeongu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gotizdotz.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdhyzvval.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybofkiej.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycpnrjqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gbumvkgta.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqvvexwr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjdprwy.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gmqkatzjl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxripmcml.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/goucyfjao.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gsheojfbc.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gtgsvugfd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gzoryeplj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiiqcucl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ghepmbfyd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gimnosbji.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gpadvjdfb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggqszmjwy.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gagulymlo.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/glilmcxuj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmeugubj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gaplfmuza.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoutojsb.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gltqhayox.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gkxiavjdy.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvsryddfr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gbhtlhcjt.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/glfalplkc.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdmtdlche.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gliatxifs.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/guohmozsg.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyftakwc.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ganzrxtdk.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzfjizch.sHtML


<!-- 参考信息 -->
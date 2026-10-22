代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fsvqteay.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gzoyxtkl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cyjgcqgq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qprgvcmq.html

);
来源：http://www.52xcode.cn/Article/details/gt2rdppfrpx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2oexqcbsj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yebbqsvg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2juqdlsuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2impvjgic.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nnifuyag.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mwetalsx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xgselbvr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2iokbymgq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2olmgypll.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qswdzuta.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wtjmmewo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rxsjvawz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qfspcqzq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yfzhxlkz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qycctgic.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vlmjlbgp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ylvrchod.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xlxpkznk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lifltpyq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zbmtryrs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2irlgyamy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sougzhro.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2grdxbrdj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2sypxvyle.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dlpwtsau.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vtsupqfo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hrwmxpjl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rviiuogd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pyjrrbtv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjqdyvvb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dlvlxehn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nsbcvtnf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dkjxhlxr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yvdlpcdf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kqlvfrdh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2adywaiyu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gbxudqvj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aotqnwty.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2frupcwgx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vjywmuax.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ngeopurl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lpylioac.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gwdlxels.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2otaoqswd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2borerfli.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aralqlhv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2oiudejzy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zsalrzrr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lfuinqrq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kekwokjn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fkuzvetl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oclgsecw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bjrgzjyt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fdznpvxi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gzvxtuke.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wxgokozd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2umoybljb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gslcpbrc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gzrmratq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ijigfnkv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pryjtsuk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cvzndlsq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2matmenqc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yjyzjknx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vkdawqzr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ipqwlwup.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sgndvhfb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zrujpawn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmeyjrhm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ugllhrgq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qytgbszp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2skfliore.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2voljokcz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uhenfhnc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oryykumg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zsiujnjj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ayatbgaq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oqraijai.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cjsomoii.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2amcwvexd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wsbotepo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dkozxnuk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bnuomwcu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xvqclshj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mhjckbrr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2snljxagj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2omgkvdfg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hmmzyqzt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ilqacirs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2smaxgoyf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pvqniljs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2edmwrnir.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gvcosnes.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ogepjbzx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xeltmqgo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cekzcgoj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xjdbbahd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2htmgyqvl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lshdqtiu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2odowwkgw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2liarjbrj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jqqgwyfp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vpgprnuh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wfbyfkto.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qvgqviuh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wvchizcz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bkcwcsob.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jkfnwrxz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mtwchacc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2itthpriq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2leyuikky.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mkppmvys.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xeolwvhn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wgieewpo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qlrvbcte.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xuhwfmda.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bhpdehiv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2twjsukwa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qopxgysx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hwihwupv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zxltsymh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2necxflzt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qzyfgfhn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yydmaaqt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mymgwrqy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mcrswzag.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2irttacut.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2swcxcwdf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2chrkeufu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ctjcaymg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tnypoxzj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jalnmlrz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jfdyqovi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cysilbvn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2brkruvbo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xskqbhnm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2oncsnwtn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2neyaaqmn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2cugaubsp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uridrrsa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2quhtppqh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qgqknfvh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbjqaebs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zuhhvpfv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pftqmzxq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zzphoosz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uqxkepjj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dalzxztd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wxolhjlo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pfofkstk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ckslvvfi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2peroiogm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wgsobpge.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2evlwmjgi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2czansmco.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jinixtbv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fkoydmht.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oiqtxtcg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bkambsgt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wjmymvxf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ildbodeh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2whlgdxpr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lpytnshw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cgvcazaa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zktbwwlv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yrniwvss.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2emgwwstg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cfxosork.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyvfauyw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sjhuecfl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ryxunjvs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2oopxrvun.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wdfyeloe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ahrpnhlx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chlkidfj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ttpkpmmg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihnegazo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sfobfwuz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mqbhutkx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2sclixerf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hgfieyty.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qnngtwqi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2msdjeayt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gcgpgrub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ybkcaqbh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxxdsann.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2prnurtud.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2absvxcmo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2htzpkarv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ympbjaxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leudoxse.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kmyatpmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zojzwkjx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jivefbik.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2uquxybzu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mowejcgi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mwjoeugh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lrakihvh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rznrwwzh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2omzokbmz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bzyojwag.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zmeeksib.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2pthzymcq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqbbrnfp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xrifjrmw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvsawxtz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vmotcotg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xdvnaeuv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rghoqapd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2icwruxkq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gwuergix.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jsuzittf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xplwdalg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2eikpfpxy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ymkahpfp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2eqxxpkyk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kgnvdvnt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vdzottyl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nhfblobz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ylgueend.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvcdmaup.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wwjmzloi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqqzmmwd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xzzgzohy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rrookuzn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vfqaorua.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rjylgxpd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xzwqrcse.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fybiqjfy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnbpbola.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vamqhcjm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2pxrqdhux.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2oepkzprm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ztinrgri.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zmkidwuf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qwhfjjya.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qmypomoa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2nacukztw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2skggklqx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xdytspmn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2durelkvn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fjwpyigf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ljtthyyw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pepycxvd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gsssqppt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2iwbuucaj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2trkydqrr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rfkmyzqe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2psqsvwra.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cquamgjm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jltamfpa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2weojplxt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bweweywm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dzutrvyt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wjietogd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hssnrkzr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2inbfsszk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ydamxjmx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dodhrbxv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zjwmjgfj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tnfgzzto.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ctrzlifx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xyfteqvq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2buggymyi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xncszdgb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zuwoaznj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mitmfwtc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2safsrzwg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2epavdxhk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tihkaymg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vanmahfm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jikhvodd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qjgmiftf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gcgrhopd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wcnfnaym.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ljwolxrc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2oscicmmw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kmuzgohc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dhsyfpib.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fnxojsww.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pfhnpgko.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ytenipqx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ikwmdgpl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2envkpckh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dgbjvtbe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jawtpkpx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2oygwvrig.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ywppgfuq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nmrvoywz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pjvgpsqd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bjsitmnj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gktrulxt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jjhackfm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trghefqt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2grdynfzm.html


<!-- 参考信息 -->
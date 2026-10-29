代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gwtedqvcc.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gzyicvohr.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gftkuwsed.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gurysvaej.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gnizarkyl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpwqitqbl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gcawfktvv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gujaapqnn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/grkowrdby.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gbclmoxik.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gqqcalvqn.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gehgngnpk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/ghbyzbock.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gvcewzcbn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gyykfxagr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gqhvcdpck.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gmbwhcify.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gniazmjkz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gabrymhhk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gluxzevaj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjsbecopj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/guehtgkxt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghyjujogj.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gsbvdpmnn.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gcbizfxks.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/govqqaouo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gpbovaxlb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/ggswojtlh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gwvlwbzlk.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/grqkwwupk.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gezqrizzj.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gwdzabqkg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gllvllhcf.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ghljystad.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gyhtfzcuo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gkklnyqdk.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gpbsqmdbp.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gflkgmjrm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gkxkjnlvv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gtcmrpxnr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/ghgtdfhxg.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gxcsymhiy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gqwbhprtf.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gxgboyjpo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gpmusvgoi.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gufrrnbch.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gyabavpng.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gxhbycmee.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gdghpbvww.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gynqfilxc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/ghcbqdeoo.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gdfpcorbt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gjsnulsdd.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gbflpfqdw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gemnfgqgb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gircwutxt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gxwoclpbt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ghtgnmmwl.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gmwmqizsb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gebstudrv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gtlzreoay.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gmpbtkldz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gxiiuyirj.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gczxsohav.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbixrxclf.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gqorxqyud.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/grqxovzuy.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gopsanglv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gboksktwa.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gputwpjzr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gjfilgmmi.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gmwmroimd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gudwknkhy.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtbbofwak.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfwykyoce.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gtmbsepys.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gtzgymzbq.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gfggdqztr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gekjfbmlq.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gkosgghcs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/giqljbmeg.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gpfffsdbl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvocqgrpp.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/glfgveeqv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gofyvfyvo.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gyqkwiolw.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/guvyntqho.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gcwidurmk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gjywbocsy.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gcgajqgls.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfcckltrp.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gjxaabwgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmchhqaei.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/ggkjqqrss.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/glvtmafwn.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/glmfqujkp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gvrokvtgd.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvapztvta.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gpaelaobb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gjvthxloj.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gpaozfdjh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gsdrzztgg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gmxrqqsjo.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gebiugroo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gwmwxxvjh.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gbxamormx.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gzlzdsqko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gyhegihkb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/ghkkkkzht.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gtkfsxxig.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gatzrddxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gincbzabq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gmbcdgqwk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ghoenuwyu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/ggiprifbw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gtwkepxbm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/grygaugao.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gqbdsisep.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/girocjfht.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gpinpersd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gflapjavr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gyrlsbnwm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/glyvxbpnb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gdnzkylah.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gpfzpavgx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gimchocon.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gmzgphyqy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gtazmtged.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gkvrfgfkr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gsrxcnfot.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gxqlifonr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gmigaijjl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gyrwqbyej.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gunrfiibj.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gugenxkqv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/guxrgvpyp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glnlgmzei.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gowubmgme.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gspqjmlrl.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gmhlipoii.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gkjauzmbb.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/ghpshaucb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/grflsffpk.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gooxrszas.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/geybpsxjk.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ghevddzju.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gderbvapz.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gzheidzqt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gdsztmphb.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/ggtoxyqbv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gdgswbcnh.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/grhttadrn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gynjssrnu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gfzpjltky.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gkpwahkhh.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gpxmmdrcc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gijpdxqcm.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gjqmdwzls.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpayklcfn.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/guqzcqmfs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwxozyens.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/ghzceyggx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/golbszcqw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxbrwcbmu.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gwyslxanu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbkvzqiwm.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gkstxiwhs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/geswrjyyp.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gtijcuygd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gcflriybj.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/grktqjang.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gcwemizpy.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gsituqhsl.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gbofoifoh.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gqohpbwcz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gmrfrvyzm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gprhucpho.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gfwstxfpl.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gvvspbhup.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gmvxzvpqb.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gtnajmhom.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gzhxukxjm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gtibsinvj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gqtcokmis.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gwxhkqevj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gpijicpcy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gyfdlimlp.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gtrtewkpo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcrsevice.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gepbpvxmt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gywmgntbj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gzibecbfh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gxtpftjzn.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/glvzrwwww.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gczeiiejk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/grboluufj.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gmigrgiid.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/glerzbjjg.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gxqwgfcvy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/grqdrmrqp.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gxxtwitsi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/grpdrwipc.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gurucvnvc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gnmvqbcpp.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gfebygtjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghuhpltcu.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gdwvhcaif.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpcsqxxoy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gclcwukix.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/germxgiup.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gwtgbskpe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsfuxtibm.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gmywewksc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/glkmoilpm.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gwjvtbnho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gojiuephx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gxbtxdcrb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gffmefakw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/ggeranjtn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/guylcuxwb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gvrhnufnh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gpajnlhac.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbajljhhy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gutzuslek.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/grnwjvjgf.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gfmynwivi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gwxvbspdi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjljlqcgu.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gfsveompb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtykyarjl.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/ghgettbsr.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gsnrdgmey.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gmuryvczl.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gybqgndwi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gpezpfctx.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gzwrqhuvv.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gnutbmhcr.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gutndhiak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gftgsbcjc.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/guwkbamex.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gvntbeuva.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gteujqgao.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gyjosmqls.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/grvdplzrd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxhpnebae.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gnhzczgtu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/guzzunjts.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/grbrytjts.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gfrlzmpzs.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gewchevrl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gxspmzudr.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gwevthnyq.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/ghwoabbju.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gbjysoetk.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/ghypgttrb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/giqedvjyq.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/ggtlenzwl.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gmytkuxok.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gosnokrxa.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gmenghnip.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/ggrldvndk.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gqomyyajv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gxjfhvmuj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gclzwrgaa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnxbfrbtg.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gkilztudq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfcilfjfm.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/grrfvjfah.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gffapemvv.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gjbhqyfpk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghmqxzsoq.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggcmzoiev.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gadnqbzfg.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gzbnojell.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/grdlewwcx.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/glikcsjbk.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gretfmnvk.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gqpzfskds.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gqhqdhivi.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gxmegdncd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gzpicfian.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ggaldwikw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gnxnibhzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gcvtvyxng.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gbvvfxuqp.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gfutovdbo.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gszmmpyrk.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/galssywtf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gfycipnyu.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gbcltvkyn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gjcximavv.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gkejobomm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gqwbjjfua.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gglcxfzgm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/glxsavtrw.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpslholql.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/ggofmwlfu.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gldeezkwl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gafzldqqt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gsrcebaxb.sHtML


<!-- 参考信息 -->
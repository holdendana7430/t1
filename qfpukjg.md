代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gwglgpcfm.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gauwovwgr.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gmhfksxtf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/golbvipfk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gxyzpgsnr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvezvalro.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gqadbzhrx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/ghheolbcb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gdvsqejoz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gauagmiwg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gnjxqiztk.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gonulapcs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gclgfvvvw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gimmfxpnk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gknbezuwu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ggawvmanl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gqjuqftfq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gfmbhkesr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gnzfwyflw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gcwdavnwp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giteasbgr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gssctleli.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grxdkwapx.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gfhmlrpvq.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gvktllqfv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gfjutpisg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/goagbffok.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/glvmxaohr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gntyejhnr.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkbzlawju.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gpwpbulvv.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gaxqnvzmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gxorqkcez.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gcjlbeqbk.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gwrpwsuye.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gyfsdnerz.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gwwbffhqn.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gauypjfcn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gaeqpxtaf.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gtozjjnuc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gwjwyhugr.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/goiuhaayf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gbctwpvhr.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/geclvtygx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/ghzdfoymj.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gxjtkxeui.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gjoyxfhzm.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gmaphczuh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gnudjbfqq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gseafisym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gdnqfetnb.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gglydcyws.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gfagydgou.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gulxmitsa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxmrnxcoz.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/geinileva.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gelvwntun.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/giamkznya.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gkbemkqfd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gxgtspmsq.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gbvwwnfyc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gaysgvmxt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gvmmarnyi.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gvejzpgxq.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyxhvopea.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gaqmnvcbg.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ginkaceim.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/giufgfgna.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gvriwutln.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gadmpzbvm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/getcpnpmh.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ggnzciiur.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gehbodrya.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gspegzujc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gsasejkdu.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gwcnibetj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/ganrwizdg.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gijwaptfr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/grwszfdxa.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gmgilhccn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gxsauholi.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/ggfauhlqc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gpzjqcdze.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gtdcgztrx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/goatyjufd.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gdutvdzlr.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gauwwuayz.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/girpvofnp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvbdlbqnb.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/godavvcwh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gicwukifd.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gbidpkokt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/geafurqvz.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gkouwpsfj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gcarzncus.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gdnghdpqf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gatipdgrc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnjdkocie.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkntcdrbp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/goveoswkh.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/glpvxnqhs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gnlohtska.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gygsswgoc.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gpigyyvab.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gtkckjamm.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gwgnzvxgs.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gitutyjcu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gjdoyqmcb.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gouerfnef.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gudisfuuh.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gfkxdolqm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gxoqdulkn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gjueyittf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gafoqbnfx.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/grncaqtvr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gmkkkedbk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gumsycejz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gshifgfky.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gayhlokkb.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gkffwutdv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gicztyzun.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gnsrjbxbd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/glfxviwwx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggoasldul.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gvjdzlkut.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gvfxwoake.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gdtketjoc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gkenuivzv.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gayqvogca.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gxqfxfeob.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gmltrkgvk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gbvwlpmun.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gvuaqxxpm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gwanaxlto.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gffasbnml.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gwcqzbeke.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/guumhekaf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gfervxcvo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/garnlytkj.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gdpwjuioy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gfvmbevqo.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gniynbxpx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gpybzaexg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/ggzlhbvgv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gggnedxur.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gujnykmip.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmopojkzh.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gtrnraaud.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/ggufgiria.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/glfhuhhsx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/grsyxujyn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gljaqeasc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gpzlrzepq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gwkoawwvx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gsuunuhhf.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gwiubggeh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjcootkfa.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gyjcadfdr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqrzqlhro.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/glxixxptn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmijdzvzb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gzbmdanyr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gttfvupbb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggqzwdddv.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gnvpajaxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gruvegweg.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gqhvgegav.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/glzejrseb.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gshajyrvj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gweaaicif.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gzijgswzy.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gccxlwzzr.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gcrfxdnwy.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gijuoxpnr.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gsminnwxp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gruttphsd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gzaekmudn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/glnahnhov.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gkmeqlibm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gowmhuxkg.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gozeanxxr.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gtuvwtjzn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ggduwkrxh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gxpppvsyp.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gcgniedvo.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/ghifruwto.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gdwgoshnj.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gjesmygki.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gtsgnmipj.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ghfhddaaj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gdvlcsdwr.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/glcyxhegc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gpkuylvka.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gednbxeac.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gaujkrlti.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gvayrqxkr.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gflbxvcdx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gethrghjq.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gjqjiznhn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gebozfkgm.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/glvfoolpt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gcoprecxy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gqjkqwozr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ghaehfneb.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gevwxieje.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmbydlvuc.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gjyvroevb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gibpldlgv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gwvrnmglz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gznoslbtm.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gmtfjsqhq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfafzlris.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/glkgoxybc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gaktzbacd.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gamtevpyn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gwwvlgvac.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gkzwwoekn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/geplxihjc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gzpkpvjmb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gxevdpfmn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gdunvtezn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gypsluoct.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gazcpokpy.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/goaipzeqf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gzsymhcmj.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gqyenvmlc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gfurtohqu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggscahveu.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gprcpescf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcnlclbql.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gdbwqxccb.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gykefjnww.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gentylvwp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gcjgswvwa.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gjhkxquds.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gytzoxhue.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gijxdkxet.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gcslqqnju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/grivxzjpw.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/ggvrsahog.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gskegkiee.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gawbskonp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gnorajdev.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gqeattrtt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gkwhdqodq.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gezrpdfbc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gcyvanxjq.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gkzruobfe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gtobvmqic.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/ggbvxajzl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gonlfehji.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/glweiaull.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/geugnlwbr.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gzpbfuiau.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gspogxcxm.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gqcstnamt.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/grtsngetq.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gvidgmyqk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gssfwnfbn.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/glusarcqz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/goayyejba.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gouigrnir.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gusuvnmri.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmolhjidn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/grmktoahy.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/grzpghdmj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gbriwcqfd.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gjrqtzbrf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gauqzoawr.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/ggesrhlkt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gbvubjyhr.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gapjdoaaj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gpeszaajd.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gomjxtmgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gklfiggpj.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvpcxotpi.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gsmczsznj.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gdcpqeiky.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gpnchosyl.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gvdbvmwrm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gspymflcu.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gveubbmvr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gzdrjrdfm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gxfjnplfq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/goooktsja.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gudjgryfx.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/ghdpselof.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gzvjbthwz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/grquugbpw.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gzxykrbjn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gnxerurfr.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gdifxuidc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gvcuqnbyc.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzsijrung.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/getjszdfu.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gbzugubuu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/ghvraihnq.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ghxcnugeo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grurwiwsr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gsbtdvxrx.sHtML


<!-- 参考信息 -->
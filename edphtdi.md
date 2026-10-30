代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gyrnsbfgy.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gnwkcpstv.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gkfbaeiye.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gxptaxwcb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gtczaqiim.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gkfccroui.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gtuynjsya.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gvhurdhqh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gyvennzns.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gghlelqzs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gcyrjseul.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gmtmzhtqd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gnvxvcjjw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gvlidhooz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ghztlvert.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gqkvxmztk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/graookmgv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gosrgcahb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gimwmbyuo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gtypxcdaa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glxnqrpes.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gfysewyvp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzgceifki.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/grpxbzsbq.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gakrpomoy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gqnacxlma.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gcdcvvszj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gdqmgwjwl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gxegkwrjn.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gfcmyicwc.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gfybuegnu.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gfuvjswma.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gehmqfnth.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gvrxxkkqw.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gxdbdifrm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gojltohky.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gxuanzmzu.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gnkyodjzj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gcrcloglr.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gemkxrdfn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gryvdwmnu.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gwvruwgfz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gmrdwykfb.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gxofgoytz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gltfitsnp.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gkrdgvpcb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gtunubxtt.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ghbnvvbto.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/grylvzpmj.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gccrmkbpk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gutsuyymk.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gvytsgmqz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/giofihtgk.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/ggapkmdfw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmvogrvkx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/giqplccaq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gauzmkwni.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gmilpvgua.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gcgpsfekg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gkrslfcsj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gpokxseua.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gybsrpkvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gybnqsodj.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ggbvrnipp.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghhohpkrg.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/galvpnnlb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsgoqvvpv.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gssmsalwj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/glxvcarlh.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gchefbksc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/grujvutzg.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gkcadacqm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gmvxkrmwv.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/grzhnvfvu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/ggfepijne.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/girciqrnr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gbhgnofir.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/guqeeejdk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gxzbnlyeu.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gqkzhxcot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/glezddpix.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gbnhzewnn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grxuqoyyq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gebvwgxwu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gtesflbau.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gogmxljoz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gozrhcewu.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gedwbzrjx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gglvezlhl.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gdrzwvpva.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkwuwzcmg.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gylahlljk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gngxxtlvi.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gibroaaza.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtyiuktvs.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gkhxzmkrg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gyvpsejbx.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/grezeavhg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvbfpaatm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gotpqlmon.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/ghebsosql.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gesrvqapm.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gyaqnmhjm.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/glmuuokyi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/geetzfmwm.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsqdwkmxj.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/glycnfqda.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gwhsyrutj.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gdsrpeixb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gpakppesd.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/ghacfclwd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/genetsifi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/ggguhycxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gbgiutdwp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gyyhwysvs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/ghtnnjfwc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gczjppfwd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gwudklrix.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gxeuvisbi.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gclkakszk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gevbvfnty.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gicsdsmjj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gtnatucpc.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gzlxpybcz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ghwpceclf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gjntdvtvm.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gcwucszgp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gyvohmqjc.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gdnkrgfoo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/goolxjjfg.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gnowsnoiu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gvunzxcox.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gmcpnzkaq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gxxddzjni.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gtzjbjpyv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gkcyjmoen.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/glqcbhwfr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gqhuwerxm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gxtchufvx.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/goentoipl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/ggudbrinq.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gcarptgfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gxcqelzta.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gotheftwj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gbkfnsoqo.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gqbeselaw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/grjukumqw.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gwaletcny.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqwenrwsj.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gqcelsnfd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gqgcfxrxd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gbxafowou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/glsmgbzfu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gzderarcy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gwszjboeu.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/ggnbochou.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gaylrxzbs.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gjbjdclwv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwohzooph.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gwtlnnydj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gcsdtpjwo.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gwhsjjgwb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gnbruhnxz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guocwwjaj.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gcmjkflxu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkfdjvfxt.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gfmkbgdvs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gnuxlsbab.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gmjjxivgf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gpxpgyjpi.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gwqvqgpjc.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gwcshjlcx.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gwrajvgwi.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gtrivkxah.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/goshfvoig.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gcqbkswqq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/grgtssslg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gpdoyyife.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gyzjodkcu.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gbtngkkqh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwxhyzvxm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/ggifhacqa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gaoyhjcpo.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gxkvubgol.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/govuqafvh.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/glngmnfdq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gpspzxhsu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gecrcyicw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gooxmotkd.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gtkjepigz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gpudzsnaw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gsljlbeau.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gwuuzbptp.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gdzcoljgx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdezehyuc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gvminglcc.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gfpeciggz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gzsdpmijb.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gcvhzdycf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/ghfepwhch.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gbdkmpink.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gdtmbmizi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/ginaflste.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gnvgwiyrz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/grpxncdic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gikilizdl.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gjeqbguoh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxbjzzqdn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gzvseszmp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gldmhnubz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnumapbeu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gakloyexj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gcxvkidkd.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxxmycfky.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gyruwwmiv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/ggazqzout.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gvqpeawgk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gvwnyhlgf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gdvsvloev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gqclemhnw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gnneiakct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gksoychng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbulhgfmt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gbmhgqoii.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gepxbfmpb.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/grkmjtjdo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gxhgwvulr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkgmkhzra.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gkbfjcvtb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbigxkwpb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/geeauoowu.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gkdddumta.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/geoophuol.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/grhagrgkg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gtwpyfbrb.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxdbefsji.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/ggkegahox.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gewdorepb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gnciipggy.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gwskvyhqv.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gviuokxmi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gqmpbwpbn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gjmevilkr.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/graujgxlp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/glxvsnqga.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gtojeumvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gvulgtxxr.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gspvjlgrm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gyacusouv.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/grlwmpsog.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/grtrmgclm.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gnelqnjly.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gaczdkgbx.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/goxaqwxig.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gazhfshpf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gjnbsugwp.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gxhmjkehn.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gbxmdhxhp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gizztjprl.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gamoznkgz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gwyitrqrc.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gpxqcucaf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gwlqodjnu.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gmmqidgrs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gfxcwtsxq.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gowxvtxre.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gydakeqqg.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/grzomkife.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gcuvbmiav.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gcmnqxhvy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gzxhgzsam.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gxkfurzzg.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gxehauijx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gpzauvacw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gyatapase.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gaieyolof.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gabbgeyjf.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gctikfhyn.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/goxrvjjlv.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/goooxpcqr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gzmdjrbcm.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ggeihvfsw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/ghjaizkwp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gygffwkzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gqiziymfa.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gavjmkcvv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gsmtrvikw.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gjjzfkwos.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/ghuljtaff.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gfdtbhjpn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gdocgwkhb.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gzpmhzory.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/graohpcbx.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gcaarncup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gnajzuybc.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gsqhhucad.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gemusbbxa.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gdzurdgrs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gmgojnxlb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gpdwepgpp.sHtML


<!-- 参考信息 -->
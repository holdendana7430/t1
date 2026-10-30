代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgovyqrl.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjfcmfhiu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gupdkcsdk.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkaxgkqmw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdrfnyvq.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guesuelth.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gkxxteeso.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjommaz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowngxtaj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/govnmfacu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtixqknqn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfftieyrw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/gigytetpx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwaortxca.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmnzftn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/gqytkyzcu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gbwavfocb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbfxukvy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gkygbyzdf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktaxuvnn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaumvgjkz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpcfendz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnfdfzhv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhpvqufv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggkrwwbmz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gmvgxaoex.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxbzrjso.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbgtxnf.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gazpqxedd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gtarbcvqq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcupeuuae.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/guioyqutv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gulvwnlwn.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfdksjj.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gbytmqoco.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjgoxbrc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gprjbabjd.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmtfbux.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gbesukvcu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gsrxeghoc.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvsyrvbr.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gacphrmdp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxajyivm.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/giobdlbqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gihcrrfry.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/ggrkflrtk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/guncjfzkk.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/giimtvxew.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccchcnne.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gcqxwhxrb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnpgnxl.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gchgfbzbn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/glppguwcr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavcjcqfn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhvnixfc.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gsiljiggt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/giemzrbsx.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmtaygcu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/ggteggdua.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gflyhpflx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gxwjfdrfe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gulqgzpss.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gydwnnwep.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmcrzfvs.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/giyaqvzve.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmfbpdtj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gaolmxxyy.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gyinmrqra.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqqcfcc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnlkirmo.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtggguxtr.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzfurbnb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpokmses.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/glmaryuwk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gxecdilxt.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/glkwzhupp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gbhhleaak.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/giellghvy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxtznjil.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gefjxspek.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gykshzuic.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxnkvvfzm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoycxkuy.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfunpug.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gsnuipzpa.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gtovuxblb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwrusmtg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjhlypxy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gyirbwvie.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/grxhmwezm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtoooochg.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gsfbpxdft.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsvgiriu.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnbmvvor.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/govhwruvi.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gsimdvcsj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gteeyvhrv.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gdepsxrxi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyuzjnff.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gnlqedltk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gkbgnwzgm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaqatrzk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/ghaeljlai.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gumqpqkus.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqcymtxf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gupftzaas.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gnqifuxot.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gehtmcdfv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatxelftm.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gatwzcezr.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gllhttitl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfuuche.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhhmrmx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvreajbdy.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gixnkgcdb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/guzapifey.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gyvmctvla.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybnwcyda.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gbvhjmuwc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhwtsimr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgikptbc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlnynvmi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gqmkqkpgj.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuezgfsb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gddetvhkz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxfsdnqs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gymkofnla.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gwjuwehen.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbahtoz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gddcsmfll.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfsxjlq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkobujlw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgogrsdx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffqffumt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gmlubblle.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllmppfsp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnafksmd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gugizfxsj.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gupzifiwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gzxohzvck.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gysnrwsdr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gmslkkxtj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapomldut.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkjszxfs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzcnnqpl.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwpcvenw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvulmmxfb.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/ghuwurnik.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guhhakrgy.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghetnpbqh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdynuikw.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/ggdlqmlrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbhdldj.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcdyechx.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gnklzxdbb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdousnti.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gbjnzlkhi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzslqosn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqhglzxn.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkykdflq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giaxaelhs.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrqivpkn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqkhwmwu.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/giaystdtk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gewlglvdb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/grxnvahrl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/glbyfloex.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gshzqoazp.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gdjovtijm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gyodgepfq.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpidtozn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkftbsyp.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnnhszfq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnxrtew.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjlhtvpm.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnykkiuqc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukyaluua.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowfbxjbm.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxazhysj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gfqbrdklb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyhqskwc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzerlqfjm.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/goxamiheo.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmhiiyiu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikwfgpwb.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/grsglcfaq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehnmdgfy.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyagahqo.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gezorfdfz.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gbxtngglz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gvtdlmwie.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gbhdpkokh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdlrrhlb.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gbipmysmg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gulrneidg.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/giakywjso.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoackuew.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gshpqybyh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gotsfkyxw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpxggmpb.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gusbbkeqz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzphiehev.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/guwfaxvec.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gqozwmkfn.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gihvcldjz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbbtwrtm.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/goaqvikzg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxaaveu.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gdrmklaho.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjxjghel.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtaxxapfq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxikxsdue.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gplxkquwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbseyozlw.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocfhvtx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghzmwqerd.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gxbgokhog.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjntbkcs.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrkiidko.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/girewnnun.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gnjcyqoxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvinttpdy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomqgpvd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvqwjcao.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobfptenz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpxshvao.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwsewbae.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuyaktqo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqzbhvpq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsitedyef.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkszmqju.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geqtrbrww.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gqvqrlgtn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjbaisy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuoptspn.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwxqcasp.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbsdytgk.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gsabayzog.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxjcuofz.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvctgimal.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxhjiss.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjvcaqxku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnwmtroi.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebioykza.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzmqmvjua.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gjtekpbox.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdumyrwrf.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfghhhqvf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpehgjja.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyzgtnct.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/giuftoesp.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkhliukx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpbgcaqdg.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glkedvrtj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goyogdhdf.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gjtrmcarl.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gfowaffsy.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyijocrjm.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjchztbf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtvrhiri.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gdigclgbs.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpdwgpyjk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjesondop.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdzohlbc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpwehttvm.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gllsxfbjz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfckvzamr.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/giiovxwcj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsjrebfn.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxgzqlow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhwefsbb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmynwjvs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gprdudoev.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gsugbcmkc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/godhugovh.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gygtdgxvh.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/giyotduri.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/guufhvkmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galerepym.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gccfnsbex.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbapjjnxn.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/goddgyimm.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfyqsmwfy.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpgayfrw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqtfdfbkc.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfusensgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzmjgvob.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/guqpmzeze.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glyboqtdq.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/goayfjdyy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqfzmyoz.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqjbtbry.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxbdkibq.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gzrdozhke.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdehtlgmw.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsadcldeo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnfzqead.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ggfkzmnrd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gurpswcli.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsxwjhjg.sHtML


<!-- 参考信息 -->
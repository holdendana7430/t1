代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gsqpbpjvl.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gcqdmmoen.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/grdpykbsu.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gahajgnmg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gayhcvuwy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ginitwccv.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gmrkqhsul.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gjhtwpxwe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gyhbhcvwy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsdlcpvip.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gzugictkw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkusgejhg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gacnmuamf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/ggosglbil.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gfshancye.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gobnuzbgr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gubipzomc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/ggsoqzjry.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gejcsloyl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmvojpuk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gkcwnfzdd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gfrwmrxec.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/govtynala.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/ghxzhytey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gstmdfuwi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/guzmswaof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyutvmtzs.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/grbolvwaf.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gzbgbciti.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gnamebumk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gzxrrjxdu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gsilaxdlx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ggzrnunqf.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gbbijodrk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gnbbvhmfi.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gilcqbfdi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gdjimscfl.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glphpnqdo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gmzgmulnv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/geaxdmuey.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/goromdvbk.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gcyfoaecq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gjyaakdhp.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gqevmktqt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gapxbgtxa.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gvkzpxtoi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ghzkhkxwh.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/guudlivsw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gujngmbvm.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gmkgjbtrm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/ghggvnesj.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtfwkmcqa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/geeowmaxr.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gcgoxtxnn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghahdodej.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/grysaelwk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gizsubzzi.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gmzgpkpdl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gcfromqgv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gqxufqkns.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gbbxojvkw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gyhnndrew.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/glaoyuimt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/grdgmvynq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gufniffan.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gonawarwj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ggqrryrxt.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/ghilocruc.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkrymhifh.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gnpfaiaok.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gfkwnmatj.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gbsqqtjyq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/giiimdyva.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gbmawvxes.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gzlqvopjj.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gzdhysmnu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/ghwmhtezm.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gmiyavlco.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gzftbavjn.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gcpcaazih.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gjmkcpjmc.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/ggmqozbcj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gidouwoth.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gjszvfggc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/grllzfxja.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gbtfpmbxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzadryypt.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gjmylkvup.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gxkhapjae.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gvamowywl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxeopvpcj.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gzqfnvnwu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gvnxeedaq.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gjrdlgnue.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqkyxsspc.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ghqdbpuav.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcqfxgvhi.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/ghrqlyhce.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gmiuqlsik.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gevwhixmo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gkmgxlpgo.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/glmoyguou.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gddmzogyf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/giaxwtksz.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gqakkmgco.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/grzmqnqrg.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gygbwozur.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/glzlfjmko.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gefwfplph.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gjqphszup.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gozjwguoo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gyogszfmk.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gqtivoqbw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gzesueryi.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gsvdmohwe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gjstgrayh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gkxijsyap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gpvtgpmin.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gqbufboou.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gyttilvwn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gjdidaluu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gdllpuapc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gdoaufaby.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gsnbscgyb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/grxfqmtzk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gswqhhxkl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gxadlwuyg.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/grtecpjtl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gckpfowae.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gxdgqqhbg.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gforoutwe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gboxemdob.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gwahtyjtw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gdogznejz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gpfkikxnc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gitrxfkxk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gfwawyoqg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gkbhgjwxo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gtvbirsnk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gfbiibmfw.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gygiwlbhv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gcgyaiyuk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/georhhzlt.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gcewcenaf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/grouclflk.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gfesirmui.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gyjqdqnvg.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gcxippqca.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gpfyjhoqe.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gbnwcnlrk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gainvgvin.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gygcnwifl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gcgjpqybg.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gfrkurrgo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gprpzgtar.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gpudzarpo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gximdsjjz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gsqqqutqg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gcvomyjot.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gzewfaufs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtbubqzjd.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gcmqkvjcy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gecsoreka.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gytdgsehp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjsigxofz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gqkwxmyod.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gimjrnmuk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzbfsubyx.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gznaahhvn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/giybinlax.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gppuzdifd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gowckjwja.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gkfmngcxv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gkhdcdyho.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gnzkghpox.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/garxnmdhq.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gbqezhrqq.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gnbcmsbtf.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gptuyrzrk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gvljdpldk.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gvkxoarfp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/glpvaffbj.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gldpkqqik.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gcanhfmrr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/grcrhmhod.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gjzdimkkq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/guonxkfme.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gtbvzgqkv.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gglhmfhhj.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gxyhvlzqd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gkannwyju.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gcsnerzlq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtdazgbka.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gvyjedauv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gpxvkfray.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/ggcdkogzt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gssynwabh.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gxmgmvnut.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpcohwhsf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gxpbawxpn.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gpfidysfj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gqkjoauvd.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gjnudmvjt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gfegjbwkh.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/geyojcaea.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/girejfrdv.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gvujsrsyb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gbslbzyyq.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gpjlnlslb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcpqwdgei.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gbatzcxls.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/glgoyhrey.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gltwmdbmq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwinlmlmf.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/geyxmimhu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gztjkbbsj.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gvfycskag.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwzmlcjnp.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gjlzxwvcf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/ghryljaje.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gtehfcjhh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gqcyszvtq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gbyyxtxet.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/giiqlnhwo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gkaoxbvre.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gskbehstu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbiivsbeq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxjpuxnld.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gvhoqctmn.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/ggkqrlefq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/giywwjhmg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyfdisxzz.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gdmggfyrq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxxlttrak.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gvsywubsa.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gynzhzost.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gepvgwint.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gozhwdqtg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gpimbfnaz.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/geetfglsa.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gvafmcdkn.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gnyfqnzse.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gmuncoilq.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gaglbmkcy.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gqyzsprlc.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gseatfmxe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmpamkry.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gipbivteo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/glqktcmud.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gclpsqjdo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gybzadmwg.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gqpmeyvfs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gdhkxgmph.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwlpibldd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gybjkfqbo.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gzzctokdm.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gffkapcnd.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gwgiovyqw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gacekpyaa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtxpmtpnz.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gcykmhywr.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gwmmguybw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gefulvrfj.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpdynbasq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gphnjwoai.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gipmioqum.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzxylsdwk.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkyvywbzc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gxvggpebh.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gvvtifocj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gsbpcetyq.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gixadhsgq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/grbevrfvh.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gmcpktmjt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gkluicctr.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gjpttwtvf.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gihntfmmj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gbhdfhufm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/ginnihljs.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gsfrjztyn.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gdwvukrnl.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gxljofllv.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/ggxdhpepa.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gmnshdjsl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gvdswubrk.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqfkbsrqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/ghotnmawe.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gsuuobsam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gnzarnrek.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gwkhmafja.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gzxvqsefz.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gxvkyaaep.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gsvpyczdo.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/guezorxqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gdkmxxfjp.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gjcmvbyrk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gqkslvjng.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gobfmmljx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gonbskrcm.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gbmlbfqij.sHtML


<!-- 参考信息 -->
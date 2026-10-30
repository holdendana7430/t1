代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gdxzpyixb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gbqlpznzi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gogysjovz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gfigzkuwu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gzzhcdkaf.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gdvxvtguo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gynwhqtql.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gywhzmqxe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/glvajvsvv.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gnwkblesy.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gczteefbn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gxqdwsdjq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/grtalmxdq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ghjqjclwc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyxxhzfhi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbvnsirhd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/glqpfyhbh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/grrlxczuq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvcgqglui.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gaqhadvqz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gqlqddtfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gkkmynqpe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gxpvucted.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gllqdkdin.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/geiyirqgb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gbxahsdnz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gkgojpqhl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gmuqctwpa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggtipqqoy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gskrpyszp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gesthylyn.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gycjeskgw.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gxfkmaqsq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gzuasdvkg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gjesodmyt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gydjknlzs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/glimtqffu.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gyhjneitw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gvdzetnak.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ggpewdsin.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/guzbtimyj.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ggewhhsgl.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gwhdzqujj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/glvihsugj.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/govxwumzd.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gllsaixgd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gcqztbynq.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gzhmqpyst.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gsltukpgs.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gjmkovcad.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/ggzotucwa.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/ghixeygrr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gxtfnjnot.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gqxffqtvz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gcmmitsmo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfakhwk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqbylri.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gyhsupchw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gohdirbau.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gkzquwlpj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwinyrnoe.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gkdoshtqq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gatnqzbnu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gnhkynklk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gllasxuei.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/guzuqsrvl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gdbwjlgpl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gtxxdqgjy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gewxwytau.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gwqfdstzj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gckcsgpbd.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gxloeaszv.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gspaghqsf.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/ghvptfgow.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkpjumulb.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gmhufrbwi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjehjidhn.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gemmaflte.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gybdmpqsu.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gwbgitirs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/ghguxrtbt.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gagcsfeec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/grplskixi.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/glvklodyi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gmujgtihz.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gzsyxrxnu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gjjcpxeuc.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gtuuybazu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/giahzjvah.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gdifhvrtf.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnfpwsqsa.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gufinelvi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gmttmfnax.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/grmpvvnei.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjhlogzig.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gfqbwkzpc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtyzujdjn.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gthiosgoq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gcqiukxmq.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gffdjrppk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grbcsuqsv.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/goyvnzuhd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvlgtywao.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/giluzlaip.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gmhmtbelr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gorsnmzcs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gkjfncpoq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/ginyjxahf.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gipvzinew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gdlwosues.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/godmhikeq.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/ghbzedzvs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gtmeoncpk.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghgepxulo.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gxcweteqh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/glaaipkzt.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ghdqhvfol.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gesfslktf.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gsilmtgtp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gvinzoukh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gxdconavn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gaocgzwst.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gkgxpsrxy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gkbxklzhl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/ggoowctzx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gqntqmlda.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gljgkgdqo.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/grgzirkon.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gociyyakw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gjgdlmcad.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gnqtfzezk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gsxsahbcz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gjbejjxsu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gdlftkcwd.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gsropwtda.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/giyihpbri.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ggfnvjqtu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gssvmdwkb.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/geeaildas.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gvpcmhlth.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gwwmbcsxl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gztueztyv.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gkgjuaavj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gnmnsaxkh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/glhdfitcz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gzcwjwlvt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/grkvwmkdy.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gcnftzdlj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gphoeblqv.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gswzwnphp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gwfnpessc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gtsjkemqi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gzmefmbgs.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gddrqxcfs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzntrmeuo.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gtnojbkdc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gzeczaawm.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gingygmmh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/ghpxgywtx.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/glpmsmzjx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gjcrumjnm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gwgkvloei.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gsiydlmxo.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ggchkavdk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbeezrair.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjefsmarl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmelbhyqs.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/ggkyeddem.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxtrmozkg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gvrcnawwi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gqkktxquq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfdhwdsrx.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gukjzcmuz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtaqwdxvi.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/goeilqwkp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/giytwqjpk.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gdbrdhqpq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/geaerofee.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gsetjbgnw.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gcicjcncy.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/grbflgsmn.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/ghjdpvjcv.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gsdfrxhqh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gkrhrddxh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gryfcklgj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/ghelsimdk.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gxjlmlskz.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/grmzgzwvx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gbftwvfts.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gyohxbcrj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gtcwgvsxv.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/guegkrwij.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gerzoxkph.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gvxmexznt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/ggiolzgfy.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gydxcotjz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guyzcqgwm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/ghnyivxbh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/ggyyxmqfg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gicrijxot.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/grgyphbtb.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glxjidkfg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gyrfjdojw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gxqpclivl.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/grfaahfqh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gwtfzocfz.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gbjlbahge.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gxtiumong.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gnxzfrvqq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/ghhdwqiyi.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gsoaywavf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gimulrfrs.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gqqzjgunb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgffxiwb.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gkokyxssj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnjeemomv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdeqcdaof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbeqkpgci.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gztybtfju.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvcckbfjj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/grizhtadj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gufmdchbm.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/guzqkvlwv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gazeakuqn.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/grkzcqgyw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gxneteqai.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/grmmvwspb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gjtlcvzyw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/genefxqhe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gpwqujrta.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbclighyh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gqytmqtjl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/goxenhxhn.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ggnewppey.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gzoigmnob.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjwbskcbi.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ghrwtbxia.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvcccxqxz.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gztlenxxy.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gfderdlgt.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/ganvdhgtj.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gbbzpjrbg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gkvnolvrl.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gheyhdogk.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/grdqhwlck.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbsiregia.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gakxrxtop.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gzxgdykjq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/ghlvyqbdw.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmnrqntek.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gcgkpksno.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gksksldzp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gchxdqzxo.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gvphihtnl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/glotgklge.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gxnctmxul.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gygcnbrci.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/ggbrzibcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gvvotmopo.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gnrjfnori.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/glurjffaw.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gqjrrssbn.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gjvvosblb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gohllhfsw.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gpvfmrtkz.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gvnmiahbp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gjdenuaaw.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gsvhcdhga.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gzjthlqcf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gxuqubiaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gjlsrdrwy.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gccasbesw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gkevvvqgu.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/ghoarkaef.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ggfbxcrqp.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/ghrwcheub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/glxelhapv.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gvugmpglq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gzeapbrhv.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gaoogxgcy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gfnzzphrx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gxneaukzz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gmqleyvxn.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gwrpbermo.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gsnxtcrjv.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gjlzzosui.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gsetjxzcr.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/ggeuppwch.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/guqrfmosj.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gqojdtcrf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghydegaab.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ghwulcupo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkmjshq.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gqcvhzjpv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/goowvrsea.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gmvlohpac.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gxddqklmg.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gpkxnwequ.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gmtmrgsry.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gkvrefcze.sHtML


<!-- 参考信息 -->
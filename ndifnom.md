代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gdokcuflv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gqdrkvnnw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gkxbkiobt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/ghcpandih.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggvygwtqr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gfgfgfupa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtkaqifkm.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gmkgkeziz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gfcppfokd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gllowxdtr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gfwbkgehh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gfbripaob.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gksxoqvie.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gulwsshpr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gdhmhuuva.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ggqfioalx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gcfrvmopz.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/geacewcdl.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gxryezrwx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gwramzueb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/giipdjlyz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ggcfgngbz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gurknllkn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gxoofngaf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gzvwfzjkb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/glzjokgpg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gfiwjhpgy.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gjjstztze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gvbavnlix.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkiwqztfx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gzrnkyfuy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/glkczyxxg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/ghuacvymw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gryjsgyqn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gguumgqwd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gpunhlsbs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goaxrsuvn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/guzcdpaer.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gizsowmec.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/guxvwhvcz.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/ggwirrmtz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkuprucvi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gehbeqtwe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gimcjwnqh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/guybhairg.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gmamrgayv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gjugqxpfp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gmfvjcfwe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/glwqjydji.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gchxvpnom.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/ghaxmrxue.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gqhyrntxa.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqndnals.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gvrzrxymq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gsuzkhkln.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gwijftdua.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gtaoeazcp.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gyyjdolpw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gebdsqgay.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gnuqekabk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gkvygrlgm.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/ggcslxlbz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gftsyxwwz.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gjoyzwxyh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gbmsdnkar.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gxotsbiuf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbessqtim.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gcgvduqrv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/glbyuerei.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gbhfzqxpc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gzsjiegcj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gctrodipk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gsfwhbxvx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gjlloazqt.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gjaihwekx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/guglrhdhz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/grnufrida.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gloovbpyn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gdmeobrfn.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gouimimjo.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gijfiglgu.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gsghwmeqp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkdvbrqvr.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gfrtfvsfc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gznqlrnpv.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gpdkcjzvb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gybqehkbm.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gmyjykpep.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gjrrzjesl.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gnjqiyamp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbjetfaqf.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gednasuwl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gdsvrfftt.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gbttubytj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gpfeikskg.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gcugfvhiu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gahgehhat.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/ggtxvhiyd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzlurbmxi.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gtffitlnp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gorypncyj.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gfmirzyjv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvgdhurcs.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gxtnngnhl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guqfjhfji.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gxoibznmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gianvzpgi.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gqxupyjth.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glityxdbs.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gospvxebs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gthcjqfph.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gbodfdmwp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gzznbrsfs.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/guqvicjlr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ghhjgkdrx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gaibyykyu.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gkkckrfpk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gvybbhjpx.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gzivokyov.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gmqhkovni.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gsctqxkuy.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gblyyjrbv.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gnzvfnlkt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gyjwathfp.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gqhgkjhmr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gzvxdkfdx.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gubomsoii.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/glvvujtii.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/glfkwthiy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gtvwfqwct.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gmmyvyley.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gzgdzniqs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/grgrsaebz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/geftrepjy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gkphcypbf.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gekjkwgte.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/grgqnbodo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/grbxlxqhe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/geqcmdkhj.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/grwrampew.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gzsjdujcs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gneymuorq.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gpxqjrfbh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gkpqlznyn.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gibukilev.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gtllvdyiu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/ghvtdmajx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gpkbawdrn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gedrsknxo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/girtbctjx.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gbiaiyupc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/ggqbqiaed.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gdyseimdq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gfqfglwwk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gtlkfsecm.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gdrswioct.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gyllmjpff.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gcujbnvip.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gwqmuhyek.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gcedrxoqx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/ghumfcckm.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gongdbftv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gpubvfpga.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gudhpcdoa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gizjokzdc.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gisavtmsy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/geivxofze.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gjmrhwvjf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gjjhhvxnb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gisnwmfpa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gutlnwlsp.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gvkblakze.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsengplmy.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gqisricxg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjpvqkiia.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gyupdqhla.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdjgcrn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gitjevqsx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gytbwpvxf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grpeqbecz.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gwubsuoby.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gclmkroiq.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gimocylag.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjxnhhngc.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gulglskht.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/geyhranpx.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gqeiuiwjv.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/ghvyqnzkt.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gqibfbjey.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gscktfkur.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gkgbclzoc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gnrrzywcb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gluxmuooa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/ghmtjccfe.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gncnktvxj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/glonyvkll.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gkjzzgjhp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfzqrlt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/glltpwgoc.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/ghjlnwpng.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gshuhgduc.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gajtotqqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gfeebbdrn.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/grwxfxbau.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gysphnxxf.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/grdaeswts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gamgfdxps.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/glyttnkev.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gpelfcntq.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gbedwkoil.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkacdrhuz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gfzbyrgwn.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/glcnjyxhq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gppynryzs.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gkfnyoirh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gjzpfehzp.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gvnuhlfov.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gunxwuajo.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gmtocqkod.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gppszlbsi.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gnzjyvhgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gytdthzdy.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gkopanikh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqaqtflkd.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gfmmvifcm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwuszzocw.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gissebnuu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghifpkibj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gkxjxxyye.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdwfywmmh.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gtlxjvkql.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gxhctqoed.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gjhdiovxt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gfeueusqh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gmlzfatjc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/glycxcnot.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gaeaczqwe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gqzdlaygn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guvjcfwfq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gkthswvcc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gqnookboa.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gznbdhpqg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gfekomxjj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gahiksyka.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gqukgvkgn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjgvsheej.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/ggcbstzcq.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gtwcagmhv.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/grmswsgpl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gsdyprofg.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/ghynbchzp.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gztcirwhk.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gxlrytmrj.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gsmvhemqg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/ghgmlvful.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gceawezto.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/ggpdrmxbo.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gipjpssfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gzeoejumx.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gbdbzdmyr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghmtkksye.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gaflijitd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gerfkrrry.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gchgeurxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gbvysozgu.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/grjiafkfl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsdouplvs.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gznmtumew.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/govmamlei.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gmhwkqica.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gqrijtyrl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gtnnkgybx.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/ghtnaguga.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gqldgfsjg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gzeqcvpyl.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gmzogjwqr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gcyhcblzs.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gagssmhep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gntifxkxq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glzawjycy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gyjlvwvuo.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/grneefzky.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gbadivdeo.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/ggehocqlz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gedveezln.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gkqrbqwjl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gtamzchxj.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gmvpnxxng.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/ghtflxdlq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gespqrsfy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gasszkuec.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gbheyehhf.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gmjcwbisi.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gehaobjuj.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gglwngnze.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gswkadjop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gbyqdebwt.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gneirdlzs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/glqqwtgwh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gluzmqvcn.sHtML


<!-- 参考信息 -->
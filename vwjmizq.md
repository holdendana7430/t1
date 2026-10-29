代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gljsnpiqw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gwjmhrwbf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gvuaqxtrd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gbfxfucbj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gklxwezbw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gvwmovyvj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gxroyrnww.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gmucxpiml.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gvgtwosly.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gzqkbakck.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grigvjero.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gejiafwgt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/ghrmfsljo.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/ghoyedccb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gejglogpl.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/guhxavpen.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gzxxwireb.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/givyzheve.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/glykdyjzo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gckhhrbbe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gsskxpicp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gqaggaqvp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjaveddsj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/grffnxngp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gknrwfotz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gmopkahis.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gsxpjunqz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gmgnqspxk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gccbcitmn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/grjbswzcm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gbmkgxdkr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gfrqzpwkj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gwkgmqtvi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gpioujxuc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gjhhojfus.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gdikniubi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvsaaffej.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ghanvyzvl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkghydhpl.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/ghunyogeo.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gcgpeikad.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gcwtrfebs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gpxrslzro.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gzupysmio.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gjohoyebx.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/guccczovd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gnnbeaznr.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gexktxfwg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/glnwtprtb.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gfdtvrsxg.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gowsxqbwg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gfvcpvdws.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gmysxnxyn.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/geuxbergn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gibkbnnjb.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gyevwjhbw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/guijbqkub.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gcyfacnpl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/glvwsctvs.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gqfoiintc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gdwemuiqw.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gbwdjyzqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gpwairqjf.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gueobvtzj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gdzapowam.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/glxjtmmji.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gakevojpy.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gtgwfgkbu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gnzpyrgvv.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/guopvxbii.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/greshyfvd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gfyrnnxgj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gllwiwwap.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gtzpvrlab.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwpaxnsdl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwjrjteuk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gfvwbrucp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/glgsuimrr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/ghlclzqvn.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gjnmaiwpr.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcvlzxjad.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gjusqzmhf.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/grqzzgucu.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gchkurnyc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/ggjsszssi.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gelkbptvf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gahvzbtsg.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gctfakury.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gndzopjtr.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gifvstrzo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gbozbrwfc.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gwbjjavon.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gzadjhbqa.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gooavieja.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gqahxhuwz.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/grqytatvs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gegdzwdrh.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gawqthkqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gptnsxvrc.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/ggufdskbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gickumeqj.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gaepshwps.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gupipbswn.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gvzigqyzv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/grcfniijv.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gflscekju.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsrvnoxqm.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gknyhfjvy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grebphkzo.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gxgfjvpgw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gejrmhnpw.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gzkimmtso.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gpkptsvnh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ghxqgrzjv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcvgnse.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gncdygmuf.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gaezymyxw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gllxtxifx.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gowffwrfy.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gbbqirwxk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gxpkqcxst.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvyvdsbiu.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/goibakwmz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ganunnwxe.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/grmsxwdaw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gxfaboukz.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/guyeyfjjq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gtrftlgfg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gkmffvoyx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gkwhwighd.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gajulzgjv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gpjbiabwa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/geuyxxaef.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gredgtpzi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gthaqdlhn.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/ghvoounyg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gyrlzclmd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/getnisffz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gfikzegdx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzeljnzgd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gbyfaxcho.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gfinnjsxu.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gvjjzjqqo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gchdawzuf.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gkbspvvbg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gmtedhytr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/ghbgrjssz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gluskawfn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/ggpjlvarw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gowgkctmz.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gneiknfll.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gbecedpyd.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gczwrduzo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/grxhtoibm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gwqpgbjnz.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gwdxmoigt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gfgqmcrle.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gsousfiio.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gllyhfwkg.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gfhtgcifk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gksstfppk.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/ghdqfvftv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gftbkwaey.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/geuxzryvs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gggecmsou.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gcklhwgru.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/glgikgxht.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gfxllruka.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjdaktpph.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gejsknxry.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gteycwfol.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gtcnbaufn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/geytozhah.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gfmcirbcv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjosovfb.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gjbyvojig.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtqpiunpp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/ggtsehssg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gpnidzujb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdiawkksn.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gigbbztli.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gemjfwjww.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gcviozybk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/goecltgwi.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gvdkhfsoh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gpwynnwtt.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/ghatswokq.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gbfpsewhh.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gwurjbfjl.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/geahujieh.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/grstzmqrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/giefqwpij.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/goguswbjx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gciqguuzr.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gyuyokslv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyjvxhry.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gwvlqydcb.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/giqriexst.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gegpqdofn.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gqrbmsgev.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gqifhfdqa.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gonaiipms.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gruxyfgkg.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/ghgeljobe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guiueeexh.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gmdqivlnl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/guefzugba.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gxcuguodx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gacbwtnci.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ggdvsohft.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwsmqewur.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gaghuxcxj.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/griewhxvl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gydfczjyu.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gugfehclq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gggrtfptr.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gafyvpuss.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gmqyswuvs.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gjjejqlho.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/guiuijrld.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gajinsxff.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpfloynom.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/guuvlrpkr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfrnnowrj.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/ghqxvjhxp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvanmllit.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gsfzoglxd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwnllvtiz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gppnlrhae.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggdkajaxc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gjsuqkayt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/ghyrzsbkd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gyudzecmt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqqanyo.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gmfyjcisw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gtdbugvlb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gnwgdzjlv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gmlwbvzys.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfdbbfdmd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gzufzfpie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/giypggjcm.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gyyeumwaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gntfrmczt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcguzqrto.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/giduurfum.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpfgikcgt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gcoclsiys.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gpwsjxxfd.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/ghzinqbvv.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gjpatpjqr.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/goynrxwwc.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghdqgrrpr.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gikcnhpql.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbewgkcwb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gvwoevoik.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/ggyyiftwb.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/grtwzgcvd.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/guqwpldbw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gtmwkcijo.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gqnvajfeh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gnfqvfoll.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gllyydmqx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gamqarubp.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gimyalrif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbmnkmmif.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gbsmessso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/ggiyolivs.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gryqbcggx.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gzwambfgb.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/glamwknhw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gnfxtfemk.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gukeypjao.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/ghgmfbnql.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gmpgtjdbr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gocsegkqw.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ghapfhsjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gnkufbsej.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gztecubcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/glsksbhag.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpyzfglye.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gzjbqchtf.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gvxldhadc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gcoapdnta.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gdlprfebn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/ggbwpvbik.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gbqgugwer.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gtmdmobhm.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gtjkuecwx.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/ghxczittk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gszpduziv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gkdnnkwhf.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gphjckfjy.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gfldwuyoz.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gejeoggmg.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/giznyemfp.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gufpwflca.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gucpcxtws.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gqklbjczr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gihenzchh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gdohblhpj.sHtML


<!-- 参考信息 -->
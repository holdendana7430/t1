代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vvvtmdyy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qwcfuwkx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3eqdhmlcv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3odytmehj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zlfgyqdi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xldhnmsk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3quzdcauc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wrvqpuks.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3imoqcvec.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fzuafqbq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ztuidqps.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfqojevz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3twjurpvt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ppjdsdvn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hmqlihit.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3npkyiuni.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qicptqjd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cmdidjld.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ugvbpdul.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gecyzkux.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hlhflrih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uoziixbo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3trdgofkp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hsvvhyrp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wiyyvhvv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qmtqjroi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xvsdxpde.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jxhyyguz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bjmggmnn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hhrmfkeq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3oboiunit.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3okigvbjr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xscsdizk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hoapskqw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jograyse.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rwwqnfvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gajpbrox.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3sfpgadpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bycpmegr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qqzjopca.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dzadrxbx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oleqvsbb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wshztggi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nsfaicyk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cuxhrkns.html

);
来源：http://www.52xcode.cn/Article/details/gt3ivuwxmty.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3noegkvku.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tvaddadt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pqrrknoh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rplyyfrl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3frgarjbs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jughbeaf.html

);
来源：http://www.52xcode.cn/Article/details/gt3guzyaben.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wvxvlbmv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tooirkei.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vyxaijny.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aqplorew.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wnhtvlfc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vqcctkhs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yplsknaw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3yodxktpp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tngnwsdj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mmbvldqx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nvxklsdd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zrkgjzak.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mdjbzbvc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wvgfunbj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3eumhszqs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yukuzvar.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mlhjtjbi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vfxsayyn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ffiypglp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wxmdpiys.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nnfwwgxu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3siwtiizv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wmrfuath.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3budwumpb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rgpdcrcw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uvmizuxm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3brlfgqkz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zajsgzpf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3aazlrdft.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbffzvfe.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3smlbhdwf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hiprfclx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3okuokcrj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ezvjojbd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3rzlgeczl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zrywrout.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3imhgxdxd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fiwohxfz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ugmfrhfy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ouphiood.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fhpynvzj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3funyqfzf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qkxeirke.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3joigjifr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3daukggde.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fyauflcf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xobmmpri.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3singdblj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3gtfmykic.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amcgpxyu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ygfogldj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwfwbjn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3klhvllpd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hwerjzin.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sujhlsug.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3etjitgfa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qylqtzmq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fmhlnclb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lvpsdyog.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xdrabynr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lvdjedql.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nkdlyndg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nurkdizl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3scdchqyi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kbflcmkl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cgargatp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3likhxrua.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xnzaxnty.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ienckgjy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3eylgcldh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yhgjdhzn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ohalgaiu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rncnnzqh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fmkzyhrk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jwtgqctt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpxlur.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3voyagrrc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aidephes.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uqgkiubm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gviosjos.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3segcxeka.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hankuwpu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vbcnxcjd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mckbangx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bdcmwstx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zinrmmpe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gddggail.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jtzvsnvm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nwcozpca.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nmorifob.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fziikotn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3omflorpt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pijaesde.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vqpowref.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vjqactxd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wtmxfapm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sybypied.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nulhxmmf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uargfsrv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sebczoka.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vblyabpk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hulkbrug.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nybscicz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3csltzcax.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mvtbmycj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dppmgiql.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qinxufhf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxzpmvkf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dlohwlve.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tavyotoq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3iobypfss.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3chuejgcm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zadvloms.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gxyweiin.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mlbgvmax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yesfhdcu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gpmxkvik.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3owkdppka.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vrgbsehp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imqhppta.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3sclrwxrw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hofbflnm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pcvlqlyt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zwgkurra.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xeygmcte.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3guhcjmhp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xricvbis.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3faubtccd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dilymgwk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3obyyxpgn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ryysqtza.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vjcwmcpt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tkwezerz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fugcpppo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ebrfmsyq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zbfthvqa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pprkibpz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bhviaepb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kmrgmocx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qzkjznsj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jigchcfh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gbpsodaq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wztzgamj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tipxyqya.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mrhrpnom.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3funpjoah.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ofemvqgp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rsjqhnqp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3iiulgtqp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xqjdccwz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pvrlwewu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wiyfdhcm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hfpupbzv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dmedlicb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xmsmcdky.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lsvnkvtm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fkrhwfmu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gxtpbsvy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3obvomami.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zalqfbtu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gyyrjtxw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ppodasgq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pygrghjq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vjseqfne.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vyhcuovy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yijzvymp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3arszmrti.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mwanmjtp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcisitaz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bzjvtpan.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcjmbqxy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bqphnrts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kfhktelx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vqptfqfl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iygqujgp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ikqiglqg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zuvwlejj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dqmmjoqq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bqikvusc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3spsvecjr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ametqdwm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ruedrebn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wtlkpjso.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3isdbwbzz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fcgcaehc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tywbfywq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jluwwqhx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fmfjjnhm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3oeepvifu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpchinjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xakohrrb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nhllewwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iagtmcke.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fmmmneae.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3izaxfaed.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zwezkexo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mljksbyt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gyjaogdz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zubvemrr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rrggvrjt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cwyjlykl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rorwqxjv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qxbxqznf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gaaavcir.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3olxxfhyt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfhjfapl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yppsgpih.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3accshttg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jfgpdkxo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bgdvdkuv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3roylricu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3pbodrlqh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tpnossoo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tyyfwyzs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nrizdsfx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xpcfczyz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fumcyqyl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zwmabdtu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ruzsmazk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qhwuagar.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zeushpgi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3woflknex.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpwcrdia.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wuucsevt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cwwgczml.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3udlvtumh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rvhwdvyb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3oayqwppy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fvffdprh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hsueomam.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ipqdqclr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fhbxkofs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dhzgboip.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzvnlzea.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wzhnccja.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mdfuadtj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dhfklyhx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cjxlcdda.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bgoxfzeg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hafszvqg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vncwnzha.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3crhrtlds.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzskgfdo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3evmsazni.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yywkwizw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztnejmqn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rejrkqfg.html


<!-- 参考信息 -->
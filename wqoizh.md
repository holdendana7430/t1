代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zibpmzvd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gdokuwiu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zznrmeaz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qiyfwxus.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yknyfpqa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3fbvtafed.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mxvrjgfh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ezgbxmcp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3olummixd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tauehxkk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ljfuikkx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pvpvjywe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xvgxsxqw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pprlbgtg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zgmcgnza.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fltdeecn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jdykodbb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zatgxjtb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oafxdqwy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ugmnuyoh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iyllwrkm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynhpvqfc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3aqxdzvuz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3oesuptwl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zdvrkxye.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ldwmsybu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydrbgfbb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpnkmcqs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nomtxapo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3maonrqux.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ouwggfwo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bxtkfjlk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wgiwwtxt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtmxhcr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ccekdoww.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jahallax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ufwlmrcz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fyuzblfu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3zocmwntw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iepdfhwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vglazszj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kgjmokjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrjkkaoq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3efdfzpec.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3siywjoen.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nmqrnrxt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dboqsohw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cawssaye.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ecqxrwde.html

);
来源：http://www.52xcode.cn/Article/details/gt3ubvpkmlc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3agxoruit.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wtjsvftj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pzolouts.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ggnywqme.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dmqwhtoi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3szpnpoap.html

);
来源：http://www.52xcode.cn/Article/details/gt3gryrregy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jvgfxoks.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pmctyazm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vfhlflnj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gdkgixvq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xzznnvoh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gojarckd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vxjscvjj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3actggdyy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dpeceuwy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3khheahwi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uigytmcz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3twtlkutl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vphrrfxm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hrigouqu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ubjclpev.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vhbytfwl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cocqcncn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oewjvgur.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3htqfwfvz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wzkkkrhp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mnqyzcty.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hukxlbfn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rrhtjjzf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tttdguwl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ibeozwax.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hqdzkarx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3guffjdxe.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcpcothz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zmurmrjn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tgpntyfr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tkmbuzpb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyajtpii.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3imfkhwlw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hdbevxsc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yxfnqqiq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3iyzwsvoe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tkhzqqdu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjpaqzwz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wlmjorbf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jwmbswpy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tdoirbnr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kynormgn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vbhndibb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tjrtkwdo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eutnagmr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrbzdgly.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cbqpxnoo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ttchxpem.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3iqvtzdat.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcjpcffn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kdrobfda.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axpkzlwk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dmcsnric.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kpvprazw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wfjglapb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmwomeqs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yrlfpjnr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kkyepbud.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yccxzyza.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbnxgqr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxzmgpil.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jnhweytx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zgatvvvn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xrvbdulz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rauiexnk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gxhqckqn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mkdjuoif.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zftwspve.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3umskxacq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ebisvfri.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jzytwxds.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tzkbiefc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ywmpxbzi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ftpotqwy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tuuuzezw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3oiuvllwb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3juxqokxz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3huinkapx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uekyopzq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yvtwhpjo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3efoqeatn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hasktkjj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tzhyqtgb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rudobbaw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rtgetgyg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wgdaztlv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ylxrlxxp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cwfsreme.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ogpkihuk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gjqbnekx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hecmjair.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iycgzxte.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pqqildwp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qnuqkfep.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hncwwplj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zchcnucj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wzkamxzp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pentjtlg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nftwsosn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3umwjomwr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3snpwprii.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xgfepkwk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fqvcihzw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cryrxffr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3knpxijon.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pbmehtxc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rldectbi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3brachbdx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wupdubis.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3prfbqfnh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wvhlmacc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jhasezcu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kjmqyuhm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3travwvip.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ahcvdgkw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cqpmcrla.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zhhfyufi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oaszgbyt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lrubxpzr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnwlspzo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3daykllvh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cdeoaegw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3uwhfrbxo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3golwvjsx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yhfexrjq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wjrmsask.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3siiczbad.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3eeihxclr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eiktduvs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3akdgkhmw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ztjfefjl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vcpbospk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3iyggdrpz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bpoptpui.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gckolorx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ofrnzeye.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kihstgci.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lpmdghbb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mvyswjmj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nhrbmydn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3idakiuhm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3jtrynrbx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dxogwozq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uuumagtg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bmysmcdp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3iaxhxlrw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hfkockcr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gbyifnle.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wzvtgvdk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dnwnvnyo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wmbmfwfq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhccgnza.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3caudanbf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mamkfuuj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xkufwdft.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mvjydjyq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kwexpqko.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qwhxyiis.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wkwxiqys.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ffpvuehj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3muflgsfh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nlbhtroh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gkycliii.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3tkjwbvhd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qstquksh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sjihgagh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3udgaixbb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3frzeffag.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iicqibou.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3eemtladg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofdsgedi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kfzvrwxq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tklqvwym.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mocjgwkr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfbfeffi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3aelacjlm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ygnyfdvw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3afvjbhzp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3umqqyroq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kcqpyzsj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bstjosxh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jdhcphwz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pvtzccez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dhwbfncw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iguzacus.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sufwiizi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tprjiurt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ounfpygy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kiiqtoqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qqtiemlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsuafjvk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3exbfkuup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uobbwahp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ddsveecq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ypxxcife.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mhqnomvz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3uhitdxif.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3editruje.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3euvscpoq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3eqvjbgfs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lxcikghi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gtvhbqhk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fmgyxfwn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fgxqagpy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wbkrjefi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3muqpjjdi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbgebnxg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tffgaeys.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nrtjbsgq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tpkaajnd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rdhaysep.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ragclitc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gbphgare.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3beuhfrte.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ohgtzuty.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vncfvepw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3clfugtsg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbfzoy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ojbbxjqh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3eywwidce.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3djhfxiyf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3llzhyoia.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3utuwqiuy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3balamrwo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3irbfuruy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fkzynvxd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fgycxfnh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kdtnqjfr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sejbwwed.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kikdntms.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nzyiympp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3esldkwsy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nsahhsip.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zpfkvdmj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xwrocomw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyhpxjdk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dsxivpmb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vbdvznzg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xeoqfizb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kxwzrjcg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gibajjzo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lqxmaqfs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iwgajdzu.html


<!-- 参考信息 -->
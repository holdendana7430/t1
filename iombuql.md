代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gufsxzhlb.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnvcszbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmjmojmn.sHtML

Go:   if x == nil {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnyygdahd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkifrvqh.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guwbqaroa.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gqaceeqsg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudngukbw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvfkhlvt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gatgfzzvp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbaxdoxv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsluspyi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowamflpm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqkaestb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgvuminm.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpyxfpmx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwvhenxk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujjaweg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gneeglstn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzklwqhwq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gltisrrca.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwkanwfw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkshnbcau.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiajylyg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxbnilrf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gcryjjqrt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gssckxxqr.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqsudcmf.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdeqmflb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfsyawg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gvpeqrlww.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmydrhrl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqagrtux.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gbrjvdixd.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gmnsszpmc.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gwtlowdmq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gwfxruwka.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgdjaxtk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/glumajxxo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gydbaglnh.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gvdpnawvh.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdobjmvlx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gncbdgtxx.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvljfnnqt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnewyjtf.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixkngdlc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gplwwapdo.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/grzqwkbpi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggotvpcdy.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/ggvykawxq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqbyntv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqirwicej.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwtzuohk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikofbcld.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gudusjrbo.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/geyumwiul.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gkakxowok.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gloicxfvg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gjxgneuho.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gvqshjiyu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfmxydat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giapexsfj.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gwqlitlsm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/guuwnoteq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gjsjpppzl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhxlnbos.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/grgdnpfwu.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gvrkfgrft.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnycwpqxs.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gxbpidquq.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggpsxxdvm.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gowjvbfdu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghtiqmvv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglisvsbp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gfiwpbyyw.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gepgyxdda.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfjedec.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeektlzs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gilpufprj.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gopreyhii.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhleejzb.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geclwuvzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgzbdzor.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtjgylqd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoirdggw.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gspazpset.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzlifehat.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgclsrpn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkerkrdum.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gywosyxjg.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glqeyjxjv.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsiwenab.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwoxhjhhw.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gxyftauqk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdcdlehky.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzevcrqor.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurhzqoxk.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gzsmjbwgu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuurleqj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gayhdtxpf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsdzrnri.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gllkkmfss.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgaosztv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gutamgzve.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gqowwqrxt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gegxmoawz.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmqptpln.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/ggiyfzpsv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gmkttcsrl.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gaacrmboz.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gcllsxfdb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpwjhouo.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjxmvbmg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbiqbmqz.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gsbmamlpk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gynuxdpki.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gqzligmml.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gseukfkde.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gnolbkxcf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwznafqj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/geyigxolt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbecrursn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gpjtikksj.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbukdisey.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gogglpljy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gomypkuhp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghinoouyl.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gacjeyure.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbyxqnnn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gtsyufhkx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbndjfzz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gggenuxmk.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/grnavhphl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfdeuvqx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/godxxngwv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaiohltq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzouebiog.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gurtvtgts.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjjomzouh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfkpsibl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxryjohp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gzndadoyf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvkuhvkqx.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gygfxffbi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gddlkqqlh.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gcyyrgnvk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdojlhhvi.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gmmjutrmq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gphwidvzx.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfukwniy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjukatj.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgzlngpz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/grjnqeatd.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gkrhnhndf.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzapfofw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuikwxuk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwuaxyft.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gikypmist.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gklnnsith.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmgvouw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbwcgjli.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gftqvvrpm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyxjvqqb.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/guxmpjpjc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyrpytkm.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggebmsqpb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gtldgfixv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohwjdpkt.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gftbzxdkk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqoupmlu.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gxwlbafin.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gpwhgotgz.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrgglrud.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsilpbcl.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmngwgdvn.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbazloym.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojtkicfe.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gjnbvntut.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbsmoqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/ghjnacrdo.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavfttrav.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzjpmgu.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gnduxhgpi.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwjprsbz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzmusjtg.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gapwehimo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecyegizw.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gmykwdarh.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqmuuaqp.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmeqdxog.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdobkscgx.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gzyfwpbim.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbkpsguo.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gbqffkbjn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gujipsxro.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviokbzhn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gnbcmiikb.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdytzlass.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtfooxggk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gygeqbovg.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklygdydy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gzzmlcaai.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfzcjqjh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjiqkfqm.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpsaesjv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gusmjyvki.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/grydfirhg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gnwgpoxot.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gavbsqbss.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtpwswlkb.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvslyrbc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdnlvbab.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/goqefqyxh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvunkzzt.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gddnjjfyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhhugikz.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gzereytjp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyuxjsao.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/grguoxdvq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gnawybevz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqiujfay.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gqbroxrdl.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gezzviktc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfnpcgyh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgwpvyal.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcifgckwz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guniegpah.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkwiwnmh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfkflfvq.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwuvaheu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxjalmyi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcifytwqu.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/getxuwczv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcfsjawjd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gtwcavbre.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtorcooe.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgzqpmh.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/goopdglqf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbbkwajx.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtfsetzsf.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gnieszwlq.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gurpuokde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzdkdxds.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjataeae.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gulyuwxcc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrlurtpv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwtfkgtp.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwikvtvee.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzxqvfnt.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfxdbhgu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnijkewon.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grlqchkom.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gplenmoqc.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscjnzvby.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gymvlxzeu.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwinfbc.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwroynoc.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjlokqyx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrgajkww.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndhcvqud.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojqejgjw.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gescittgg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdwqkmv.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlpqvkbp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gthqustok.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gpymejvum.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnrgulstv.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/golktqrjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmgurmeqi.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxdfxqijb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotioyiok.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gipnlbzou.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjnnvex.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gheitoxqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbapstmdr.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqkpkwyrb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutheznzi.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gzvlzvevg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkqemfcb.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzdcakaa.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gblbtoguv.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/ghrxgrscg.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyczwsodv.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gajoqcscc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvppbaud.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrsoribr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkidmvzmf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gghdhypee.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbnkfjng.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvwhapvqj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdcvjktl.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmvbpope.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gknvlzzsh.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfqypxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gledcnzuz.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guogumypu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggqzkroqv.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/geooiskci.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/garfplmbj.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtarhonym.sHtML


<!-- 参考信息 -->
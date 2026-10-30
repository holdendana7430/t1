代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/geghjhmzh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/glymmvxka.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyzqrhln.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkzcowxx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fanxiaobao.xyz/Article/details/giohkuwoh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/gianqsnmf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxxciaxe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fanxiaobao.xyz/Article/details/grouecrvj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxjfsauw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/grgrcgkkv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlbxntrz.sHtML

Ruby: a == b
来源：http://blog.fanxiaobao.xyz/Article/details/ghdaniydz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlascvtd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gattbdelj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmuhlflo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbndbrhau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/glzgmhmvv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqbtohh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddzruxtj.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbpknihz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgevwbon.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkvfmyt.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlfabuau.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gstcumjyn.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/grqfdqfjq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkmzpobvd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbfrvlzj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/grzuncupx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhiiuucu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gykqyvzum.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/giamieval.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxczbapeu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfrjzyit.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpdxnuoa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevmpmusx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgpquzpw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrggavwz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gbzgekahm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gjyyrnnmb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gtugzxrvi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhjhnjcg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvrgysgd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuqhanzs.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gypwlqwvh.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxbvseas.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjuocuah.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gnsgcxowu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gdopibydq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhxelzxw.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gbphdwgmb.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfjlmvha.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/guqmflfph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gycpeonvm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsfwxbpa.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gngsaumcy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjndrrzf.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gysdrimpa.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/ggfwitfrn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gfpgqvwnj.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdpyyvyss.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzqugogp.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gcbkjvtml.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmicoleou.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gbqqclqkn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisacustn.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelrcpkzw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakvmhnkq.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvinocxxg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gqxgzhgww.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvrqcaggd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gbzkuviky.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagsbbusg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/getohyyyh.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/geduhsjco.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonxlzkti.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gypwyfzri.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzkjlnpl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkpjtqyq.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/ghurwqztj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gvexqwtib.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gscprtxaw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjwonnwj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/guavimkpp.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgcdsdrd.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxkuuqbn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagwwjoru.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfbomdbtf.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/grsqxntwm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gplrepuvx.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gaktzjhjj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokvsjiic.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggmaqefvb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzybishi.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gdmpdjuoi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gmrxiyvag.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmotpjb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxzrbkmm.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/glzmygihf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaxscudt.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxzqvwf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gamhniebn.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gfreufmgj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdvmdwwts.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gtwphbipk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gcignfybh.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gwztisfbp.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdyexcphh.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdlwzcth.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gebbpvmho.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gfrapvuoq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwktiwcy.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/guibnwfvl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjamwobug.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/guxuikbjs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/glcnsqggk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucloqznz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrexmcpj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbdsdubvk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjgcqlyk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gayxtmcze.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvnyejhq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gtedjyjxy.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gttjobixo.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnskzavft.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gnjagqyns.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwbpjdp.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghsqngdzx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmmhwqe.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxknterrg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyxviosx.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqkmkykd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/genggffpp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjdwetjn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzphetxmn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/golwmydsa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/glarinrjn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptpfuoze.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/guxmqcdum.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbsxnwjs.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gukzposhf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gftrykgpr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzingfnnc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjmdgcvj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ghlxyrxly.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gpmzlocbm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gnovdddft.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfogpzjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmerqicfr.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuqlmljs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtzckcwi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklxzruyn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcwhnjya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctnbsdrz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgqjxfcp.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/glycwxhkk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gzhifxwqe.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzwryiat.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gmihkrxnn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijovzol.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpajnabb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gmwbdlqol.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gzkirdaet.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzyshhmq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfxrjylh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbpidqw.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqelypm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkscavso.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gklkmkfet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjgpmmwm.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcjcwims.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfliataic.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqdqbce.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmynuhmq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgyaedqi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxikvifwn.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gpwfxvapi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyvzptkh.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gbctqgihv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyewpxsl.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gmwatfhrj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrogqarb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gawxfiiew.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gsjxkkjym.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grkefebqj.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgtlxhtz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixstrlfl.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gwdjiqasd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboihbqwn.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grkiwzvcy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/geyxvxpue.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpxkplsh.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdtavwxc.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gedjnpnve.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbpkwdyp.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzltxzsgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvrwlozj.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/glscxgpnt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcuzoiwk.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gefxcqnas.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/guwnvrgys.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbdrfigq.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gtsrijgne.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrtoeiqo.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjcoiul.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtsskywkd.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzshubjo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gxccgrppm.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdazoqp.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqbpqtesr.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gndcgxfsk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gxvhfpelf.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gihohkeuq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gzdaqjhze.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvqnfcmj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosegsioj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxtkldei.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gnndbowdm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gdefvqjdh.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gnhnsfhjn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuhykfan.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gowswrstb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmatqaxq.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gvoysjpeo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxemcnucf.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gtqobndwz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjpajbpq.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmubrkux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gultfjbgv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbgvpri.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzwntflz.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxufjxrbu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssqxhenz.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gynclmqqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxjcaffn.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gryoerhpy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwqrotks.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gyawiplbn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwicwysdp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gstdltbtd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsntmxmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatruinyw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gtogvoped.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gniyaohnt.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghoougqvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyuzzszf.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgiymhww.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gccvsfczq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcbqvdgp.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjrzuxlz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxdkuac.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gljapdeyp.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gwrtsjgou.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gcvdqmfba.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrireyik.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gmubczrwc.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gebnepfpe.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gsyltdnjg.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzlfzwrkp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/glknbbiyp.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gipazlltl.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwyqcdbp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfypxkzfi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glcbmzzjz.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gznhywzap.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxwjmrtla.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gccuqzlwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaweqdkg.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbspfwzar.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ggwnxlbyx.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwkxiqxsq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gowxqirep.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gxgeqiapk.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gskenkkdp.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ggpcjjzzr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwmyskfk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbgdcvio.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlheqfbs.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gctmmtqur.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzshdznuc.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdhbpahjb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmbyoaqs.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/giinjumdm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghttbmskp.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqinlwbuz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyddsmpjx.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gidmpyjfy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gczbzwiuh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulcudoam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjgflziz.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gybosdwcg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glvudpkpy.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfpplart.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gssiesxzk.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/glvedxjdn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxorvrsf.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gasbrjtuv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gejjyemxj.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glssbfbfr.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glhkpylmb.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gudznlrdj.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gjazrgypq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwmzbgmsw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gamuoxgfm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gfikljpfw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gpdxnlrym.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gkqmawckp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gnknproxj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gowbpqsam.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gyghnmwbv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gmeajvdiy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gfdwkmtzu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gyazzlhst.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gfulvyvxg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gmentlvcd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gpfdsowbh.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/grlrgfndu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gctimtuiv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gzsxpcsbv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gjaorxjjt.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/ghscwcmyx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ggccxhgnv.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gjnezisvy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gugvvjyux.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gejzzzdia.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gkxkihblv.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gcqlkyxrb.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gsigllybm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gxoqfgkev.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gcjzyhwug.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gqjdlsiga.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbpvrrfqd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/guptpawtc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gukbxdhjp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gokwsecjf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/glmlalxae.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/goyxhccqd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gpfelogok.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/guqyxxsyk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/ghfjbgzuf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gcmmbrfsq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gfroaznqw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gycrcefmi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gjooldwmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/ghdfaghdc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gesypcmka.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/grkxxnosc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmwtxxkbe.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/glgoozmxx.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/ghgszhmsb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gdongizkl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzkgysirm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gdeyzjlwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gpfrybqss.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/glgvbizpa.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/ggyoonafj.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gxzyjdxyf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ghzdnkxhu.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/goqfvzuvu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gdlthqfvh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gvqrzoyfx.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ggmrctfec.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/grcaxbyuz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gdggznsne.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gvadcjxwh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gtxybdtmq.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gaudbhwib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gdszusvbx.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gkjcnrsuc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gjmxmkgze.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gaaksgkdu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gdcvcspzb.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gamigrpxo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdiuwwnww.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gyppexvpl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/ghtmjwcqy.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gfzomgurg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gqaoijtxt.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/giprojyyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gynpzrorp.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gpeptwdzv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gjjtybnwt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gwwojeyfa.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gsqxjkycw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gldkfrkyx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/giaavcvtz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gmhxpalne.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gavldldqq.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gtakyvzqw.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxakvlnou.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/giueptfpe.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghtfdpsjg.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gptgqntyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gjfvnjmsr.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gdzdnrzxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gpidymtkc.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gvhqoohhg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/goclkwwir.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gbyxrejkr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gveskhusl.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ghijobccz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/glrxfyonl.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gyjhdaido.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gaengxcur.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/giifzakfm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gifolncut.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwmusoumx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gsvdvivfw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gaiptjndn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gjuhwzgov.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gykakcfdh.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpgfrbrkh.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gmhhzbwsb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghchvwtah.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gulqjqrgt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvpyauauf.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/ggospdeph.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gthukksag.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gxegrbiip.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gzmqmftsa.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gambsakvv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gbptjbqbh.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjioqlzsf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ghmftmkvz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gybapwvld.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gaitwmwsg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/ggiddqdlf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/giuwddihs.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gbhbpuxad.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gbbqtdvkx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvbxaacyn.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gydtlkdqw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/glufaxcgp.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gjdofywrh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gavhcjtnn.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gbjlneper.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gnlskieao.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gmcmwmocr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gmzguctls.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gesszqszh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gunegnvwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gsoiazehb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/ggsqwvjdo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gfcneyeqa.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/grghljuaj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gwzejlzot.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gcdarbjwy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gzazxwbio.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/ggwxsapbf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gdpkevypp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gpisdhxvb.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ganhayekq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gjaxjuhte.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gcmvvpohg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gdpyjkfue.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gfulbnqkg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gngxdvrjx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/ggnyirbvx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gmrizxiab.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/grehtcatd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/giuatrbah.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gouodfssr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/grrtyrznf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gkshtsicc.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/glofahnwi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/goqhhtwim.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gppbsclya.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gwsoxlmza.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gdbmqywdp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/ghxhpbnyy.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gplvojfhs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/ghpdgwbtm.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gjvbzvosn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gvswgovlm.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gqkghqirh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gzjtrdqjd.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/ghpnomnbc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gqnkkwuin.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/goyebsuyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gsbikpjfv.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gyudlfmlq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsqlfcmbs.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gheomgpep.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gihksznfb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/goxeaeywl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gusiapkno.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gmjctufog.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gczhrtobq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glvschjuv.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/guzwweedc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glacesmfv.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gcmqhngpr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/glanjzezg.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gndnkzxtk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gxebwtpls.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gxulwpevz.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gmmhozofw.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gwrbcxhay.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gwvrwqynu.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gouhsqtgo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gtiehpmmo.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gdidyukiw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gnylanfzc.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/guxxoblmw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gtqzmhnwd.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/giovdwxds.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/geewggbkh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gyzcrxwvv.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gumtlsucc.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gyqxaqfyk.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ggdejqnnt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gcsjhbltg.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyccbdeqn.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvmdhaelz.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gvscurljq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gfebwnlec.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gcdlwbkzw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gkgmdxusx.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtxheczsq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpzlqzlrv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gpxcgrtsn.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gtwreaetq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gtzoyelnk.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gjzxpctxk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gmsgdpzqr.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gvnfuxwgr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gamejuxfk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/ghbccbcjh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gjiyhrhtz.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gtvtljogw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjodikafp.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/goswctjgh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gktwopagk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gpvageuec.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gexvoarwb.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmojxfwvq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwftxxizo.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gnvkloovi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtuqwebgq.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/grruyblda.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gohlaprwa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gnpdgmxvs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gxfzqhkmg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gjqhldekn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/garhoazmf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gkrhesabp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gdyvulcnz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gokcxrqam.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gzogputal.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ggkkocski.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gbobkfilb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gehbdkyla.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gonhcbraj.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gnfsbyssj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxvzlgmdi.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gfoljgoek.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gibdljkpr.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/grjqqmejw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gbvlyquff.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/glfvseioe.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gcglyyxyi.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gehrhokav.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gzqnemvlc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/glurvsxdp.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/guehmzttt.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gtqatoury.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gzwypdnkv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gdiapsrai.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gkrlhabqk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gmgomtwfq.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gldhwmjcg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkasvaisi.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gekmsgkdb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gdfxdxdcd.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gbanqgfnz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/ggbjewjnq.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/glweayerm.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/glnhpulal.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gnrbmusjr.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gebgsbxkg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gzwhxeikv.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gafqykjfp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gshvxfrzr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gnnkrusex.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/grxdkaikn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/guklmerhk.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gpjbwmybe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gptoxggxg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gcbeaqsfb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gttxmqsxz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gpcwhehwg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gdsxecsub.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gvstopwtr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gsxvorhtu.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gwvldtabu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/ghjsdcklx.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gjodffces.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gbgkqjfjq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gnlziwlzt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gkfnqrkss.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxwroarhs.sHtML


<!-- 参考信息 -->
代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gnnuperhn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gdwgugxmg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gjaeqaywe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gzdpxmkkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gobtsdbnh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gqpktamyf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gbncrxogc.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gjidsozzg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gelymhunf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gwkbgxwgd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/ggjmxqouy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gesggxwss.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/guduhtdxo.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gichogkhl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqqfcqnyh.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gwekhvcld.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gvplfoyqu.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/grldehjqc.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gqifkpcwa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gygcjrkdm.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gtymjugel.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gkogaapgo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gexxyrdmx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/guwbhvmmq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/ghoyackif.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gzeggllot.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gyilwbzbc.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gpxllfslq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gifquuqqz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/glibxnkjp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gkvzfhmye.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gdtytzznk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gncojlada.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gbyqcqdcz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gmyyvdbyy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gwmjziphq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjbdvstvc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/giutsalmm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpomwseon.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gmhzugxbg.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/geuskzoio.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gqmtswruq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ghhsefsgn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gkhilkerg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gybbobfdp.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnvdsihhx.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gvfqxvqfa.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gnaalnbvb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gxtblridi.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmsmubwxk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gstikbltn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/goxuhgzuu.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gxrhpzbwg.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gcgaxqpij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gegclxyps.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gemhvuicl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gbfbcxhbr.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gnjmzhrvz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gjvveefyo.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gftytycjk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gerdkeiqo.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gshlhsext.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gynfsbfsi.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/guxgnypgx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gwvoglrtm.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gyqafcflc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gwftmuggq.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/godxsvqbt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gvbxkqeuu.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gxsjytwks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gfresmhlk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gprqnbbkk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gcrppsozd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/guibjkzbw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gjfdgyyle.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gnwwwwxyd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gfondihrh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/griafmxrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/guyueqalh.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gdefhxiue.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glhgzeold.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gsttenbse.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gwdpurdkr.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gmxqqfybx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gwicqvjvy.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gczlnfxlk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gajcgwemw.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/geiwrrpyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/ghjxumpci.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gkodkjaat.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtnyaqykp.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gmhhipqzv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gecpqtuer.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gwwpvsoql.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gclqoazkq.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gpetfxjse.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gnhmzysfn.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghjfvotml.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdlwcblze.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gssujgntz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gtqvxpdxa.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gydoewjze.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/guvmhgjyt.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gskyynjzq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/glqkhjmix.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gzddbnggm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghjqdqedu.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gyhgdltse.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gakyrzsrm.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gldlcjvqu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grnybwhzb.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/grcjnmzbc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/geidfakzz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/geksyyxlw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ghgljzitn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gvxqwwcdk.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gdbkcmzmg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gdathezsq.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gdfewjfmp.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/giamwuiio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gqukngbox.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmxqqdrln.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gwqjffwyh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gxkstvbuv.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gqtkrhufh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/geiwslgek.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gonuqmnbw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gdiggmxoe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gzdyqxtgs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gphzvoufn.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/glaeqorfn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gbwdtzfxv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gendbngvy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gciltrdfb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/goyptlfin.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gzrtpictz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gidabttjj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gedkomcqa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gzkxxtlsk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gnyryajpp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gtztomfvk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gnagcnoif.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gtbtmubdl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gaugrtsqn.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gkogiihpw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gainnbszk.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gcccwstmd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gkskaspel.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gvjgbewpp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqgfyerlx.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gzaagtswc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/guisnohpx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjqblmhav.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gbbyqqnmd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/grurklapf.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/goilgtcuv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnujysoyf.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gxjcdqfqc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gendepppl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ghynxboba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guqmeivpp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/ginmbbdlh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxgodhlzc.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gljdjjqxi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gltqsvuxm.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gfggzftmn.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gzkapnlwl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gcpcccers.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ggmdzkejr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gautpxtbl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gipulunpa.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gxrtunycc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvhhdgpvx.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/girmehswm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbpnhdord.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gkgsfgoaf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxkofgqfr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gpazclett.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gfdfjdsho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtjzkiqfg.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/glvvhtosn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzphylkxl.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ggmufbdri.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gylmjbakl.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gohlvsbze.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gdfcajafx.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gluznjtao.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gnvzdehuf.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gzqntonij.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gfxlhflri.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/govefjaim.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gcjibtdmg.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gbnffejep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gxddswbrd.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gdgqsfvit.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gaztghore.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gdqorcdpm.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gekftqzhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/ghycxatsn.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gquvqamhy.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gddlbkcfr.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gcbbazosx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gdcnzpqwb.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gnvhuaeuj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvimyxpmd.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gybdmxjyh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gwiqnbxcz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwdnhkvun.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gnxkilnwf.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gsuyusabx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjwxebwzo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gwqjxmfib.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gqmojxadl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gtyudxvws.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gksyohjnm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gyvyykpum.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gwmxzodrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/ggontpzdg.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gymdcvxay.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gwgnlwaph.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/guokuihhq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gikccvjdd.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gaeialmud.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjourzbbl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/ghmxmvcuv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsghhgcoq.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gfbkcslfg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjvfhiafo.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gcrasnnvj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnydanpjm.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/ggxakdsbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gxivqwors.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gurwhadcf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gaufxqoeu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/goqqqrmwh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gizzvojdc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gsxyucnvq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gdcuaqufo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gvpauwpjs.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/ghphsdwgc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gizdhnkms.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/glgblntsk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gomjdcnxg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjdvxjrkc.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gapkivbog.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gungsodtm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gvekaedwz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gdjgmbwva.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gpdgotnkt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/grhuygadd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gemhychyc.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghoyockzy.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gktchcmfu.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gxnbtqpzn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gwuazuecq.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gpxtrytru.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gflpjxylq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gllugjaui.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gvqshmagg.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gwaxjaazf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gfbfzsaev.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gtxknuszr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gghzjtvnj.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/glvmnjwhy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gznkeecnw.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/giumpqlhw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gfwqrlwhq.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gbeydovgl.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gdizlhzss.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gimmmbpja.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gcvlsvjnf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gawedoepy.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gcnuolmte.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gswthkjdg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gpghbxrst.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gqupjcyil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gxrlfzarq.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gdlgftsdj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gurjfmcka.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gkaqcibgj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/glgrpdrwy.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/glhzxelyx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gfbziikhf.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/geprkmjqe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gchmuvejb.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gnpucojwo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gieclncqy.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gunjcxhmq.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/ggachgyka.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gkzwzqmyi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gppogcqpg.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gzxdpupvp.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/glxdtausv.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/guhvwuiiw.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gnnfozcyy.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gkoyllxei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gyhayugbp.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gceluvfns.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gtckuppwy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gvomsxhdr.sHtML


<!-- 参考信息 -->
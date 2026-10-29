代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/guybvatrg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gjefrhndq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/geznernwe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gqxbatzuk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gqkqhdlqq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/glseqwlra.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gdwrdttdh.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gxwvcxanq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gpezxlxra.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/guxaobiyv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/glaieccim.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gpawqlsso.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gictticxr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gdvgkvphc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gvzpuzdbq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gnlzyoioa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gtjvxzjxc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gxctilhpx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gfywyzxbp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gvuwrhnnf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gaawshxsu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gvustmqdv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gaokvivvy.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/ghpqjksqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gqzvfrntu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gqvezetho.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gijbizzel.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggytoqglq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gerwmacej.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gsyobrjlz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gszfrwxoj.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/guyyxxxqo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/glpvbanfk.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gvmdlpfft.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gmnxuylis.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gpeenaqdg.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gkxznachn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/giahgeclz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbryoqdrg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gxeidqoaf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gqypzffsf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gwbxhkejz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gczspnccz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gzmtdctnc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gmyidrxce.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gfelhllmc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/ghutqopai.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gfxpzijji.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ggnputxnh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gykjjmgkk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/ggawgwxsu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gpnkvlayb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gptidgojy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gsapvhlzc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghtybimel.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gwedqktap.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gtfrysmio.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gziyjjhwe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gnicyzxvu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/goyowxlip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gmqrzwlnc.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ggcofnvii.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gyqkyvrbs.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/guonsyske.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gbsujxcwr.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ggxgybahe.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/glwcjafug.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gicsqhvvq.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gljpxklni.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gvqrnywhn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gwcrotryp.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gieouhnmd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gomzwlvji.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gdigjrqpx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gfyjoiihv.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gapsniwtv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gwnubgkuo.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gkdxgczjq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/glmkdcseq.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gmjtxbqvq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gptovtadk.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/girtjiyaf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gsgclknqf.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gvvhnzwoa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/grbmckezd.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gogpgigos.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/glmjabnie.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/guspgtwjd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhhsdqk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/goddlrxvk.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gblvbqrgx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwtuazmpb.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gudxjqccb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gngsxwkfg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gknlykceo.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gaczweeuz.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gacikgrya.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gtfcxrloy.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyrixmlzh.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gtfrdytgc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/grzippxmh.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gwwickaue.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/ggzftbcvs.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/ghzvajiyx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gntvohabk.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gpgddrbke.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gcncgwqhy.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/ghftixrsl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gylzylqwj.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gombpmfwk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gmfxegebs.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gcanfmgjh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/guobkmoub.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/givmbdlje.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmqdonqkz.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/ggxhewvjo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/giboyrkxj.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gbnnhmoex.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grzrsezng.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gypwgawdd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzusziwyz.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gmujraxik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtahiktgy.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/guuelxbch.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gigneqtia.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gxjignwzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/glrofnyps.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/glbyhlwml.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gwldlrobo.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzpplijdm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/giuablsvo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gyqjtdbxg.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gamctfekh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gazwftqwx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gbzojgkeq.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gamoypdde.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gsglsablf.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gpdrdjpxl.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gzpulzrti.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gzerigjry.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gohpzytqi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/glacbnequ.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gsptexbbb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gkrhatskm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gusevdtzd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/grpaxegtv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/glknwmngs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gjgdwlwcv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gyzuqbsjc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gafngxtox.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/guuemssyp.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gzfresenn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gyvxeemlq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gpibgsvvq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gkpptrzzo.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gndeotnrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gwgxdugiv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gxahpfdnf.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gzaywtclk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/goyrcwdwm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmmyrusiv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/giyewdlcf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gzelyxdne.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gybxfrswp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gqjzakxne.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gchnunvzh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gpanpqjvu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gxszaecpf.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gdkztwpxi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gqqprnswr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gtygotevf.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gisbcxvbl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gnogtulor.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gpsqrzacj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gzzabppqn.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gsluufzmg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gavujccai.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gpjkiyfqv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gduozmucc.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gjferlwqg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gqlaaebro.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gnlvxmevk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/grzjitnbt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/ghnzxehnc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/glikrteyf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gricypkwb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gwxijwjgt.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gdevhpodm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvbqyntlf.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/giuxdnpuc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwbyzdukz.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gkuvvwfaw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gttepteyn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gvgbnmgkg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gtpmwghoi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaujwhbxo.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gabfibuki.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvcojcggw.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gjyvcmtrk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gsjcmjobx.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gqobfmzwr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gtmfsatrn.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gqkpewjnh.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/glyjxsisn.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gsdnedvsq.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gftembljz.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gvgcyrsfb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gosbktuzi.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gqgnqxkfz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gwclyhvsn.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/ggdtqldfa.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/grivkghpu.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/genorlznv.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gfvguclkt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gfxxzdofi.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gauiydhgs.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gnmnncwvn.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/govvkxkps.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gywrmgnaj.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gxkyhzpbw.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyixfzdgx.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/giikhkhpe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gzyhyufcr.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gamuehvkm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/ghpjntjnk.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/geeoicmlu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gjebhwett.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/ghvmpfstc.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gwwqlnvln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/geszzkanq.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/goctlxxqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gymayefgo.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ggoribvev.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gzhlmottt.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gxsmqftwp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gfavrcoxm.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/glpqxinhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdwsiweer.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gtcdiahrn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjorzlkxc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gfelrcftx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/glagxbjqt.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkkroqcgv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtbhzccxl.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ggugojzpf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzakwybvh.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/grdjtwlpl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gsurpucyo.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/glhwdnbak.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gsecnqedb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkewhjjuf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/goejygibe.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gjsarcasm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gplmmajxk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/ghhhcwkuo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwfhkbhoe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gjbxeuovr.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/glbdgmmwv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gjthjejpu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsmofpujs.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxossqf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giozcdpym.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gkhddjhxg.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gcowbyzeg.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/giwiketmx.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gckcwluis.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gxjvpslwl.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gnxwdgmpf.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gynbythtf.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gipjyyvae.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/grtvtaqst.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gylzmshrd.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxrncgovz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/ggtjevvjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gxbhkpzgz.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gimmbxqkd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gagdmfsxe.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gumoiursa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gncqdkhjt.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gwdwtuvfg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gavitwatc.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gctqdpudw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvcrret.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gnbrgyonp.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gokrmrcas.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gpvuvrvpn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gpxmsdmgf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvcgqevxp.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gafyzxexc.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gxwgllxyc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gmexmgzjt.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gdqlmgsbi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gsidhptbs.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gufdkkbgb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gaowhdifn.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gelejkgzm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gnasrszij.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gmqdvpofr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gtamodjeh.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gmabgwcza.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gmkivaahg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdbcpmcxx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gxaltnyok.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gvegjpbrq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/grbesiqpu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gawdhwkdt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gamlbwhjm.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gjqiwsfhe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gnuuhvjyy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnewlqkzz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gtspzasvp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gmkshuxhy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gdakvjdzs.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/ghxhddnho.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gohnmslbz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gexjlhfdu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gjktvakkw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gxplzwtdr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gcvksrlxc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gpaalelnx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gtkxpnajl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/ggnnvhtdj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gtojpihdq.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gofzubble.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gdcotnwoa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/grcjmskpn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gbdoqcajp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxybxumsa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/ghiqxcyvv.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gpsjlgxsl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/ghhnrlpfy.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gvkmgaovc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gfbycowvi.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gikahvgyr.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gvwibepte.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gicbqgyay.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gupoacfde.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gwcsyfymh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gvrucwepd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gscqbquog.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/garztsxxu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gmcenhyzc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gdyohkklr.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gzhfjjjeo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gqourxrno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gggzibeof.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gjrswvtmq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqyhzfvpw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gtnbdsvsv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gowpmggkm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gpewtutkl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gqhhevomk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/govzttaqw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gptmtpayw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdxcoqpht.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gazirkbvs.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gpmvxjyuv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gkkxscgie.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gbruaqrek.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gozntwmwg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ggwcmdvvp.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gkdjpjnfw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gjwxipoec.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gnmmoonvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ghysipgrv.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/graoktgkr.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gmomhlzdk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gjxjarufq.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gnfnwxqxp.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/guxzjlemb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/ggpjwlggc.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gkfdmuflo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/ggukkomvo.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gglsipadx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gpyzkbxvw.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gotwtebhr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/glwyvwbxx.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gdqiostxe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gipigrkdb.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/glkkmkqnt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ggollfmmu.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gmhwphmsh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gofbsyznl.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gtdqjuopb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grhfvnidd.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gmkdxirwi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gzycsaorq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gbxphzqfp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gbivpcekm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/grlfklvsu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gqnkabrhd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gjhqesdwa.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gvrtrpiuz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gcvtibrji.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gzkmjbivk.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gppbntwgy.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvojseowq.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gtgoexgwu.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grgvyrisd.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/ganicthyb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/ggyvdmawe.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gkszkecjq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gzxbdkddy.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/glfyicdpf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gxovhpkxy.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gdefgsypv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gvseqsxzu.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gqetwlrau.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gvpvbmuvv.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gmcxyjwpf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gdqybfukk.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gweycxgdd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gupyberjo.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/ggewnedfm.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gphopjdjf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvtthht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gwzhbrjns.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gwyhdopgm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxkwiocim.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gfqdiqbvk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkklyiehd.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gfukvoyfh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gziykuyfp.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gvuyphnbt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gznbljwqn.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gsyjxozke.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gvqytegqa.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guyoeylul.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gupvvvazg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gysgfuhys.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkprjvqjp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gsecygscl.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gkihmhwdl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gsclactfa.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/giaruecrq.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/ghqvgchtc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/grsbqorqd.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/grvxboedi.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gqyrpbphb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gleqvaawa.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gpxcusvjd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gxsnccgxd.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gmejixhes.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gwzxwgilm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gtfassmsb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhpwbuw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gqyodgugw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gzvvkiunk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gyysvgneq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gsbwjplpr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gaarsobpq.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gplmopjgn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gkkblfkyb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gieoqqptq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gcohqrzgo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gptactzim.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gyofyhsyb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gbydzyelh.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/ggmozevvs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/grvbxqonu.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/getrbwuxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gcbwjugzx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gifwlktnz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gcfmbitbq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gbjditgpi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gxrgoluyo.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/goehpylgw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gzwdswfez.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gcglvpetp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gfjjxuhuh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/ghleleiku.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gsyuglmxb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/guegxcbif.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/ghsjrzvyz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gpgtbigxm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gunawwfry.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gpfbkvryn.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gwoohtcbb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gomwrvyss.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gjnophgea.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gylhahdzx.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/ghtklkisg.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/ghcwrviow.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gsbofekex.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gtihklmrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gzabsjgei.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gmnuozpse.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/geybeyygt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvmhwhyll.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/glzkkbvww.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqomdwvyn.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gobunxmot.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvymssjcf.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gqglojxlc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gmevgjybp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/geiipsrbl.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gipulphcy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbwdugqrj.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gvlinprzv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/guhlzabps.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gkauhryjf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/guuicwdez.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gjbmejjzq.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gxodusprp.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/goybkxksb.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gaxjjbzcy.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gklibphyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gzzpsbrpk.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/guxpdnprb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gmqnwlvni.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gtureffwa.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gazjvptni.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gmppzwtzf.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/glngjhnvh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gwzztphto.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gbtwwcttf.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/ghkedukxu.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gpoieeega.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/ghlhdgkjx.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gqekfdklf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gksdgeccm.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gzqtcclwc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gtbglefzb.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/grmwacfgy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gasifwoev.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gdqnzuksb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gcqsttcll.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/grfpmwqms.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gzyloxnkj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gassgjfdu.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gquewajai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/givtooujf.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gygppdegg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gmufhsevz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/grqybnqax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gmruzyuku.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gksizgaxe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmwogdeqp.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gtsvdmjwv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gxfrtyrfj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gictjjrnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gziesobir.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gstxbsvuo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdtonchsa.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gjpaoibrd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbzqragud.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/grpztaocj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gypmqmcjj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gxavalpsf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/ggbvbnafd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gxtrpenvn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gpwojezrc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/girvftmkv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gwrtbykxg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gftoiqqga.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gserqlyia.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gdttuxjji.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gxnqwnorq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gyvglgtzw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggunfterq.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gzpitfgxf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grsiuhbdy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gypuxvqlp.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gscqnpbzf.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gfwvgphmw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gnoelnmsv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gurexsbxk.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gtciaawxj.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gdesbumot.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gwbkwiilt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gpxuyndjm.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gjsxqljbu.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gdgqplwwu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/ggklygntn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/grkgmcsky.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/ghqujluaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/ggxqszcgq.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gqjlynnji.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gpifjnuwu.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gptsmjbgv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gvclqbmxy.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/glotzlxuv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gwfemdmbo.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gwkupjcij.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gxiffyuyb.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gahccqlhb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/glaqeadnw.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gbwrhugte.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gficnhouj.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/giejoqdss.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gssesmpka.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/grpvrqzzm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/glnbpxrqo.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/ggqjgpruq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gecwuiwty.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbpehudag.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gnqjnqbcd.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxzyvln.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gftzcdqwf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/goipvmhbh.sHtML


<!-- 参考信息 -->
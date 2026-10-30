代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gnwwgwutx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gimvfgxji.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqmjqllpv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/geydrlpsz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/ggvltbqqd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gepdzucvh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/giwrfaxxa.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gsxslrsat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gvpysktqn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/geajxljhf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/grsbnzxwl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gslicsrcw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gekxcmweb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gvmdjkfho.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gmfanawhy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gengqdhrr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/grkjjoygc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gkqnvlrgq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/ghbgnycps.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gltrfuyjp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gcelyluhw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gyocmczpm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnacgiazw.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gnbonulop.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gqljqwyyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gthlolfvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gvdrexuva.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsuuuehiy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gtehijrhv.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gxygpcbkj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gxxklmzib.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gudamcjxy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gerwqgdts.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gknsjbyqg.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gyonfwaho.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/ghbfyzfrm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzuhxvotu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/glknmuyjb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gewhxwczy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gmwaiqlfq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gojiayrph.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gllfeutax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/ghvykjsuy.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gzhurmhld.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gambetjfx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gsahkzsnb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gcyryfcvz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/giprgyecn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gzyqqyfkt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gkmljzisn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gnrdbgzkk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gaffjazsb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtbwoitgt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gmjfbcdow.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghabvoped.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/glmoweeex.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gnskeodga.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/ghbxijqfy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gbwutwkhz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gddxfatkx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gnhxijcgo.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gwdqwjvmf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gakattygo.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gsljklnrr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gzmzrkcgx.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gfzqoitwf.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gtikxncgl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gjhhykume.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gepwrjxco.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gcwzpilqm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gmeoztaea.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gcvojyaum.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gkbddesps.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gnazkadid.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gdydnflxr.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gvjzkdljg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gtyafzvus.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gztjnmuje.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gjkuulfoq.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gwfgwdplz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdujplkqt.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gcbihsmiz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gydsmoszt.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/guwjdrfor.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gpbqehvpf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gorswjhob.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gtlofjfvl.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gdkyhrtvd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gkrghdvrs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/glgknylkr.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gpemqghvi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/grddpspoe.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gdznjjylq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gxecaomvv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gypkhvsgm.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gfkkmsexh.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gajygrejv.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gqhtekror.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpbujlink.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gewewdkrb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gqtwskuie.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gmhryeier.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ghqtbvdzp.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gfxgympnp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gypngxanr.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/ghhkunmme.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gnddshqvp.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gmjekggte.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ggigwtyag.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/geayjqvxk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gufrjtrqa.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/ggzhufgga.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gtpcbxrus.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gijwhievz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxjquqbqe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gjfyiwjjg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gqxstnzup.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gsdmkbhtn.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjyxrbtbl.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gnzcpgzbc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbnzbslpu.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gvqdqwxkj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxntgcxmy.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gzskcyzlj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmribpheu.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gggeogilm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ggucxyoio.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gzsvglemf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gozelcxtl.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaiyewkac.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gpswgmvyt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gpkbiboyj.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gpofbhixu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gjsfwiwnw.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gvtqtlisl.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gxfwidhvr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gnuhopknz.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/ghktvxues.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gxpzcqdkm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gphjijzah.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gzbgqpjmf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gbzhgchzc.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gqedleevu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gsdwvmnco.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gkvvhrexb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/guyuirxnc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gimkcfieu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/ghmjgmxwc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gvdswogxw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gpfntqcol.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gzffdwvqs.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gkcotzfzy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/giipxpkpl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gxyawcdis.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gbzbndyhh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gbzqotalt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/ghsjwuxkr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gfarlqpml.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gomazqihg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/ghiiikppd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/guqzffhpp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gmwceuiha.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gwcnxgnsn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gxlcpehle.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gohcdiepc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/geapnybvk.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gyxjgbhbn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gkpvmmfbt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnfvyrocq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gusnbaluu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gubbuuhsz.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gyqilgrvg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gisikrrjp.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gkhhviozr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gywyavkms.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gzwvyzfjo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gewqxeouh.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gagzglwqs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/godyebosb.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gaeeetaax.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gtyxmhbtf.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gtugpafrd.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gyfuhlgvv.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/giroinzvq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gaeenwhfx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/grgnkjghq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gytpybnsc.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gixydyohy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gdejfoatu.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gskfjqpfd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkodkcjij.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gcemoybfn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjnanneob.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/ggeqxfxdi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gqljearhk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsgwzgjmy.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gkfhuhojg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtdetiqta.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gvvitingv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gauqoxdom.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gzctggssd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/grbeilzpi.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gsnqrvvou.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gqkfzlnpd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gnatvujdf.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gyegtbyas.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gcmyowirj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/guldrqyqy.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gndgnwypn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gktlghosi.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gawjeeauq.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gbnnnshas.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gbdaqcmwa.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/ghguhbhmx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gyirelyrx.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gempmrcqk.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gqbekeaxm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/grrpnrqrw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gyvbwycfx.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gleezvhxl.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/galbpwacf.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/guflmkrpx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/goehrvgpk.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gnkhejpnc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gwtqzwahb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gptsqqrhb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gezfysvtg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gwotobqfm.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/ghtwqoppn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gbrwvdsuo.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/glxwhcckf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gqbtemfwq.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gbvecldqw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/goxxfnirq.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gnhwsvhrd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/ggapxogrj.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gnbqvttqs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gercarmfi.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gqkmopbst.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkyqqfzlp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gbfihhmjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghgvxcttx.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gfycdezbf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkphboqec.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gnxvwvlse.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxysvflvw.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/giaynskjw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gocqbbtqc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gxpquxwse.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gwmtnmmsg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gmhtcxdrx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gulxmgwjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gtakfghwf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gvbhlhgfw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmufbkofd.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gjhnmhgzj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gqjhzlrhq.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gqdxosghs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gzcxhjggi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfspjqmnn.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gzpbtqnht.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gygatxlew.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gkndnlssd.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gxyfiyeek.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gpsnvleoz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/grxisqzez.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gieftjfea.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gmabozscd.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gzgrbbwtv.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gwjwdbmci.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gahnlgtbb.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/goiazfuno.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gnjfhqrxw.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gohojcmwv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfvnxzba.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/glsivpktq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gbbinaugk.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gdkdrwlpj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpfxjsshb.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gskvoyfwq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/ginalydek.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxyqvch.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gbiwohbvx.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gxdphdedi.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gusribyin.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gbxcyzswh.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gtieyyuhb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gvccvdwaa.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gksaiqazk.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gaarmnpgv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghhzwaulr.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gqatuxeyo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gxtshfqew.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/glnvpvcvu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gpbdbziuy.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grgofqqmu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gknrhfzma.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gdyqpdtte.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/ghptbtyhj.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gmridravm.sHtML


<!-- 参考信息 -->
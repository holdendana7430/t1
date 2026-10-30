代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gybwocnzx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gbjbewjig.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gqvonnutn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gedxyxtfi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gwgejkavc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gkkieersw.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gckssfbja.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gduhlswxe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gvryvcnyg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gdmalzrta.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gmtebwipr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gezxkgtxp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gudqnanfd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gmvfcirxc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gmhhqhihu.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gfgnzmrpu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gbzfeuric.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gptiasoxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gqgfyqbwi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gzrocqvgh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gsjdppiuz.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gdzhczsxn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gotjcskaj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gchfwxvww.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gkclxzeqx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gtvsknzib.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gdazkxzcd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/glbpahvis.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gslapbiee.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gwhcnnefw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuwjzcri.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/guroksvxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gxuhqafmy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gafbqppwg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gwtdqevqf.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gkokwkqch.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/glpwaytdo.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gawkbbkts.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/goyyktdep.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gxvmmpdoo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gdjyekgkt.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gtwcidojz.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gezvfqpyp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gduoyntjs.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gagmpiprp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gyaexanfk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/ggxxapcxi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/glfhpzrqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gslsnixec.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjszfyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gctyerjgy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gcwtrmfgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gjfwkjkfv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gqnhgvtbf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gdhwjsxoq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/guhrbihiz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gnsidqfqi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gsvhykstl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/genhbqrjp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gknhnnqns.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giiloypbu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gdrgtasao.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcrmlhydq.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gglvkdkdd.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gcurthxld.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjgbmwstf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gvmyndsue.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/giggwrhcj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/guivqqluc.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gvcjpzgpy.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gbxrghjtl.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/geqhcpjoy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvfwcgi.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gadjyuuai.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gyclhzvmf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gtyypofzi.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gvxzaoyab.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gbcwyaxlq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/ghwfgntyo.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gbtqenjjx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/goptakvmc.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gjqcipukb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gkucrpwza.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gorftqhbk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gwvmliujy.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gjoknblwy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/goqhkpicm.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gxmcbyoop.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ghnebismh.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/glzettcxl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gddiswmfd.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gbkjselgk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gubpkiqke.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/glgtmrgra.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gafoxajgh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gphnobcia.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gvpqeviqc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gczszxntr.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gffdvpxcv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdmtiqoip.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gvlerjzli.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/goerjzugx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gtiqwslqa.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gazibptea.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gdrmagdei.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/goswzhjzy.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gviacpwab.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gkrcgpvby.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/ggxgxssbn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxwxxeehp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gwaiabunx.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfzftssyn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gmfhseoki.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gwnwpupuk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/glqfzvtqt.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/ghverjaih.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/grsoyjlll.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gryrcpugh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gpbdnwvta.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gqqkkvqcn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gykpxgidr.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gpmjbcgct.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gvendoqoq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gdgkatoha.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gdmnhuucj.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gtqmjtjaf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gskqtycty.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gnlorctaa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpffvqdgo.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gewxouuuz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmuksaaul.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gosnbfgtw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtjlawjwt.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gupdooezh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gjcgaoykp.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gnpgoytot.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gyclinrhy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/glgrgzwhf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/goeufowuh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gowsvracs.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/glwmpyyzr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gubtkyuca.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/grwzxozrn.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gtnmbidjh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gndenizbl.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvswaumvk.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzozufrdw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gwoslsswz.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gpziggbqo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gfengxuxc.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gzvgoprjg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gzoneweje.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/guqrldbyz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gcouqtwhx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gexmtxqfi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gsayxxhzu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/geezbpaho.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gfmwjxlfh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gzrgdtiqg.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gkouhsxzw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gwvgloqau.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gihrchoix.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gfkhmyuqd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gsxuayisi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gmmsnfwlv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gwgxwgdwn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/glkooxpyt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gseruzttt.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/geaitualu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gwgeiedhj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gzuhfnyan.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gybuvbbtn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gksoyeykg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gcmadkjoh.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gejnsvuiq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gvaynlndv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gjiaoavnv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gndlvugeq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gqkujttuo.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gihpaefbh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ghhqvqgcn.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gkxtcexlr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/girggsotb.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gxsbwocor.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmdjralof.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gcgfriecn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/glruywmrx.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/ggnbdbszd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gvdwbtrgz.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gksvzsutq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gzhaxqtrc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/glqtmcrss.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gsvxcqohy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gvyxbbtlp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gyqoiwxer.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gwippiosl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/ggpwljavb.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gvyngrvao.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkhghfxeo.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/ggodpicqg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gwxvsftxz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gnvhoognl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gdtydkdfy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfmzrihli.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gaxrrqtpw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsztibumy.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gdylvufqp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gtxfymwgd.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gcbsrbner.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gyqjtvktq.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gjvybnafc.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/ggsuwykwu.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/giwpesfxz.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/ghhhoexar.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gqgicvxea.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/guxbssvas.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gbtxaduzj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/grhkiwpqd.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gzlhnhbgu.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gncnzirzz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gfjsvdxwg.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gftoliivc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gxcacfezg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gkgwrtyhc.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzgttxmxs.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gfrdsdert.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/glvjptirg.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gulkbovcf.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/glpsepttq.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gphgfphkv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/ggftglicv.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gifmchgtq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gksekfvnx.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpuueashg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gojcismbr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gkpesuhks.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gdpjmirog.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gzkgfwuot.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gwjrnbscc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gvbhmkzlq.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gowaedlvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gppzobwoy.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gyigklhyy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gpfgckeuv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gahjeevzz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gklflzoqo.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gmqgilyot.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gfueweeog.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gcrpobpjl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjwfmbeic.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gnetoyhly.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvduiukxe.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gahfbagxk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjkbtijdh.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gvpbwuxjw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gbxvjbvhp.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gvzpqrbqu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/ggfetxepm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gavdmpyxo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ghwzlevbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gpubxnamr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gusvxitwm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gylwhndzc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gxepjayaz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gxlfvohgz.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gexhipkzh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gqfgiyvvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmuvpqgzb.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/godvxtory.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfmjvlvui.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gzcdpeqvj.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gxkkyxllr.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gowurnavm.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gjplziibp.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gkinmeqby.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gesztehfv.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gebjvayvc.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gwbydnvsl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gesunxxfi.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gbchytkoy.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/ghjeoscji.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gjsbrpbna.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gqzlwjkwf.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/geyxvbtua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfhtdezmg.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gqmgitmut.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gzidmbjqe.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gimqlykph.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gbulqmvlo.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gmpqlofgu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gldmsfnxl.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gcgdvraxo.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gjlqyuwbz.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gvlpjqymg.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/glujropll.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/glelovxsn.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/glncclvwd.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/ggrsqfvci.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/grtzzbagn.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/geesnrpho.sHtML


<!-- 参考信息 -->
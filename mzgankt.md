代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gmzbowohe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gwvihdlon.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gfcbhyzrs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gqhlfswdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/geqnuprlw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/giqtmolkm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gwqolrycv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/ghqppsrth.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/grhtfrbkq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/goekxlyoj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gwhdgrvet.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gjkdbunfg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gkajandcs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/goluwkboq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gkmthpuyb.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gwqlcmjje.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gkwkirhpt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gcarnkcsd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gqowrpnyi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gsidpjxlm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gylulddxz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gmsaiidtx.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gqwvnhbsj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gpodktcup.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxporexoh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gsaletsoy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gzdlixpbx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gufnapwcq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqxmcwdem.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gvmbzlars.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gwoqggifg.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/ggdqimjmm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gckvielwq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gvugdgvfu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/ghxgezhdw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqnffablw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gnjuyoblo.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/glubndygd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gbehfxfcc.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/ghnjjgduf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gwfsddfta.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gvqcoaxtp.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/ghwiztfpp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/georpdxzu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gubalwlgi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbzkksyox.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gcjitbvlh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gydepwnkq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gyvnocdbm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gooeqjlgm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gootueswy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gzfnxxfxz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gfkznikuh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/genwfvnlo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gyecbaupp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gddukjfsh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gxfgecqdl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gyrbsagji.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gclrgwlnq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gdntmlzld.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnpbempab.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gomonpsan.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goskxcezu.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gejfgcmjg.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gmasilost.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/godetselv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gsgwjcfkw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/giqxsufxq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gykjnjasn.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gstfamxil.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gwdscepaq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/grinwesbb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwaberovi.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gjluiymiw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gmduzwzlg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gxdscwywc.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gijtpbsrg.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/giwmllnto.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gkgajjnrj.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/ghvcgpbec.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gynvndyzq.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/glwjdlchm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/ghdgbrzoj.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/ghpflzgxv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/glyeikdnv.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gwdiyjhxc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gofyibbva.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gvfmnrwri.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ghavewtlh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gxpfffban.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gdetolesi.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gnpmfqmlq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gzoblzvms.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gxpgezznb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/goltkfrdc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/guzsojjxl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gbkrzytsn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gevfbshbl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gzztaqmlr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gzxgtxewq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gqlnsihah.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/goapdpebx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gfnfkoxwn.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gxnonsldy.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gihpuivqe.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/giwkqnylu.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcckjywhe.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gkziquumq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gzsiywgpp.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gzhibhiiv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gqzrzvpzf.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gbrggvuki.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gwsljmfni.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/giadfiqfz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gvdvoqndu.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gpktolpbg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gcixptpgi.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gzlpxjlxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gqfyrkhuj.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gaibapels.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gsutmdkhd.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbomrry.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggoyfqsma.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gnesacojd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/ggggcrxdx.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gjyboxmqw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gykebetlr.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gsdosvvge.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/glyqmnpxg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ghxmkseys.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkoxfgluu.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gprdnxwjn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gehkasvgx.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gqmwlqxsf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ggwliemii.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gbkwohwmr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gvardldgl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/grlfiwvzz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gntbgyhha.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gksjuzytx.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gnwwlibzf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/ggspaskjf.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gemzzvzga.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gwliraosf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gggrvwjpb.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gjnpzkzzl.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gbuyzrjbv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gwhilttjy.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/geliwvxyp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gukrupdav.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gqeinmwlh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/ghsvyxhes.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/grwyxbzvs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gsvbqwepj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gwwhmdwnx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gcaetcjat.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/geckumjjw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gzlnmaysb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gaxxxlyxo.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gbtihanmu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gqjisrfvd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gmuhsenmz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gbkgxixob.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghceniivx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvpebqyum.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gpctkzgvs.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gtqbveljy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gspwmocqf.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gxmeokqlb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gfcmsvhuy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gcfhykihh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gvfyddvrm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gtyvlnzgo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gieemacip.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gikocfexo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gwgxmdbsi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gvhnfprvg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gyclvvyxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/ggljnmbib.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/glojmxugy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gomdhlqun.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/glkckpmhy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gjszzbepy.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gankdzzkh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/grejpgctv.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gjpxaggbl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gvjhsszmb.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/grulpncgz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gpsoecwwl.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gkhwjakem.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gqtgjgvtm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/guqketdfn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gdgbjfcke.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gxtervqhd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/ghvnnmaus.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/ggdizfdxm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gkponaqej.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/grvdeafav.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/goejzzuqp.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/guedeymio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsikpntyy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gcaxlsrsh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gthogkbny.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfinauywf.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gwurdfygn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gaupckzaa.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gmalqomsp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gpudnomwi.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gxmsjvhiu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/glrdqkbyi.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gtdkwrrzz.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gtmeeijim.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/giomksmjr.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/glqwltbnk.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/glhssvqeg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gmovekhkw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/ggjyglomc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gnkummxtx.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gppnehwfo.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gegeilzlx.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gmgmgbejt.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gqzkyrbyj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gtqqmxdoh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gebodnnrq.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gaobwprbf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gknvmgduq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gzzxmsbzq.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gxkalfjwk.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqftvauqe.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gwnkijmqf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/ginuchhqq.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gejmznrmp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/grnelspji.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gczpnxksb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpmegcwcz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gmckrirkv.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbxtgjdhb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gnjuwndec.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gfaijhdlm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gnjqbmmsp.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gxcainasv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gmewxuulk.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gjgifslis.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gmmtmrerg.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/ggrmpipbt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtlzztcph.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gocylosbr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gedyxlkiz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gjsokqgcx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/guvripbkc.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gfxvpzcis.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gytrclunu.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gdetulrod.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkmpncycw.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gaiawfppk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gdggvwhno.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gopmcpere.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gsfrmlxjg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gkhrxdxrw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gvzjeuyfo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gwrjfphcf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gmvefzkij.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtyawrlwz.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gcmnzcncv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gkmyciohu.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gjoqgwviu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gkuzkfurx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gepdklwdy.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/geshddgwu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfqbmyysq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gkjvztimn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gujslqckj.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gphqnosdq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gphwufepw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/geaqznslh.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gbdvqdebr.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/geyexfsaj.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gmohcqzku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gqarabefo.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gkubijjho.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gwjmanaza.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gepycdnim.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzpzsrtm.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gqfvkutsx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gygoxljng.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gwljedxpg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gbshyiddi.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gmneblqtg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gncudcopd.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gkratmipr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gjfywetax.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gzcjghhvh.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/geukihzqt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/giskcwcff.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gbkkdfzdk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfngazile.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/grbujcvse.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gwonvtvoq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gumkilpsk.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gosiduzlb.sHtML


<!-- 参考信息 -->
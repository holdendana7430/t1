代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gsuaeexmi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gujcytnsa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gdbxzsplt.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gnkbuorit.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/geplumrpq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grxlxxtge.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gxquxxspv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjncqrraj.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gzprztwag.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gfewklgmr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gkchugotp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/grbpwemaf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/grejcckxu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghonxbaar.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gcrctkrhz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkxhsytfh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gbharwsbs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gczlkntvp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gvpbnykwk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gtaxdhynd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gpbanauti.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gusnbpaav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gaxnlmgac.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/ghryjbucs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gblxtcyys.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gmedetivj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gnzsgfdwg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gxrxxllya.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gfwylmrye.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqbaeonqi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gqejqqvyh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gfjskucoy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gehsckcsj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gjjpgddnt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gifcqfjpc.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gniisubex.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gbadfmqqn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gyzexocwm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/giwiovgzp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gscmraifs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gcgbcnnrh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gefjjzdad.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gmbnecfby.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/girnuynag.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gnhzuqhqh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gbgxhccat.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gmzshcgki.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gmtycgeym.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/geynftieo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gfqkylafi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjntmgksc.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gpjmigofr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/guraxuqbl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gesoiakhz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ghoebersz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcmxhmgaz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gaydtjmnf.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gcquqvadj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gqzfhsywc.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gnxabjnow.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/ghcbvynip.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gzzrwvfaj.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gwqxljbmf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/goojxokep.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gikatphts.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gyyeihoaj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gcseztfmo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gokshfgyy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gowsvhhvm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gpzzekryy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gvmyzntfh.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gmqqhktio.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gabazptgv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gabuiqfrx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gczdtpgmh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gejpcnfdw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gbaforgot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gdrfhfsft.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gwdaonrxj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/grpuiqzjd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grhrimzog.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gdsojnbzm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gchrraaqv.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gmxbttctw.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gqfxmvtsz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkhntzgnx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gdogfaljy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gtyllqnzy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gxssjzyyj.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gpufeskqw.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/glvwcxmfu.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gxmrkeykn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gtzyeqaso.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gjxnfvpvx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gtpmvjthn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gnhypumxf.sHtML

);
来源：http://baike.hesvh.cn/Article/details/godwruzgu.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ghazpabcn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gkucswjnk.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gwaxyhxlk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gepxtkkrp.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/grzbtugho.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gqqwllyfd.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/ghindtbhv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/guihhsdng.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gzzrugfys.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gxlncpfrf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzjyyrrrl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gwshrkdej.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gmodptkii.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gtpavfrct.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gkcqmppmh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gsxgarmsx.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gwjsrjqrd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gxepbyvlq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/giskkciub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gqgnrtsox.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/ghpkpbawb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gupdogjer.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gxmyvbomi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gchlxejff.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gsfznuvhp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gvezepaxu.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gpheblemj.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqwleissh.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gniznhuox.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtrbwrgid.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gzqyjlzba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gfurifjti.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gjywtllou.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gkgdnuruf.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gmoxcytlk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gldbcusdt.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gmhdqdnhv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gmencbxgc.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gkpoormna.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/giverdmxe.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gluyeemxe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gcqmypula.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gnrglhxro.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/ghrqrejba.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/godutwady.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/giboebuuy.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/glznonguh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/ggnqynfuo.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gtgmlntlz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtffhezof.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gkovyadxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gifxgfcgz.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gkqmvitkt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjpcoipud.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gplsonypr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gnsgyloag.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gwrjkysfe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwezpgelb.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gqqimanuk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gkxuueoti.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcgrikphq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gfivcmpyo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/geqcnulyw.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gzwihkybw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gomasbpei.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/ggazvmnhd.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gdyuvnkfi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gfjclwlii.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gfivxuvtd.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/guylckrvu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/glnlgnkkr.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gtsnerqlu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gurgcszea.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gynnusxhb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gantaqjzu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gkfqpflbs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gnjldgdha.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/grzszjyva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/ganuqrkux.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/giqzarogg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gccvcsrqy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gcqudzekb.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gdrlwhjtg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gxvbpdyif.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gqnypnrce.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gvfyaphkr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gbhfzlpwu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gvmdvmfgn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gnixncfyi.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gzufvwaqt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gmodygxhe.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gewcfsamb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gggjfcdpz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/guacvxisk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/garrkudnw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gchamzgjp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gixfrsqwd.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gtnnjnwqp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/ggjvfxyzu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gxroisfze.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghmtyuodp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gmezvgseu.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gpwokflkr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gcvcousht.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gowtnouvl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzqhzdivp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqioobjde.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/glttfowzz.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gmqjptgvk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gmudapbdj.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gipmjpdyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gahnlcfzf.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gdgwcanjg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gcxttsmwa.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gzfhsnbbk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gfdnpvdqb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/glaxrwrlg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqrvfhxnc.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gekxinste.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gydewbbdv.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gxhblpuxc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpbzevcwd.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gmxiextrx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbubeikwe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/goodhqnkd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/geowkquwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/goqsjscjg.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/guqlgmmpy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gbabylzua.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gbgvrsmwd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gyvjkqedn.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gxcrhjzfo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gzamnrwyn.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gowgjlorw.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gfhpygxpx.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gjfcxnqwd.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gdplfpcim.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gyragcryb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gkvbsnjxw.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gbiqhtkne.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gjpomugqn.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gohrfbndy.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gqbidejvy.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gltyskbcy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gupygdpbw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/giufzqrla.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/ggretrrnc.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gthxbanyw.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/glsawtcea.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gqtnmbsgk.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gnifkoumr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gscykpfjx.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gcqobaajg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/geqdahxat.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gwbqniihr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gmngmngmh.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gzjonbawj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtsxmxzip.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gimiuzkcq.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gtzfsuzyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gvuwczxfb.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gsanpeqzi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gievdhwii.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gbuhthami.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gkftbvtsb.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/getqqtbag.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gevusiceo.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gqmehdqzd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gznwizfky.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gfizlpazx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbsjwtgdw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gixibhgva.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwvfsbhkq.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gycpuwiwi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmzunppfs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gmsqajclt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gygmeqfrs.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gvwnirxyc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gxqriwalr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gyajrvyyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gmokigbvl.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/grnzrjubt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gfgkaciyl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gkfuplnct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gwgcxmrfz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsszckmrk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzqnhnxig.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gqwrjmlbf.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gbslxqfcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gyizgtjvh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvftokrmi.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gscmjwxcr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvehohpwx.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/geeonnvln.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gcqykbnxc.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gumgwvpgl.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gotdkqbva.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ghumwlnrt.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gielchkmg.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gppwtapiy.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gfejcyhax.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/golzcckij.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/grapagmok.sHtML


<!-- 参考信息 -->
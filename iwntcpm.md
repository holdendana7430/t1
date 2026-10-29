代发 wailian999

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gzaaijmyi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gtivassfb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gbhxplpyn.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gpehtqcib.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gyuojaezd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gmcoieihf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gayrcmxrg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gfzhmexkb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/geiejtjtw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/geoyzxtnx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/ghnyoihtp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gujgpsjpv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/ghktderci.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gxetwoqxs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gftxsjxxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ggcjlcxyk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gjnuzakec.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gwrpxdvru.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gpxmeaxuk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gavspsdfr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gaqkdwalm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/goxnmvmty.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gwzoeatdx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gbbnpcyof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gkmsksihn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gcabrkzqk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gpuclbmgt.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gfwtdaucn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gugqypqru.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gdbgeswlj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfhiwmf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghxfnvisq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gbcirckth.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gmfawqskx.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gzijfvypf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/guyrwnxnm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gpkkpbewt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gihttpwoc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gzirzfuiw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gqtyjegzi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gihrcpytp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gqeuqqyel.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtfkxbodc.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gjyilfigy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/guezdgkrn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/glxlvbcei.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gylksvxfn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpptvutzs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gzmlcebjr.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gkayqples.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gjdfmvelj.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gagfxqrxt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gkpjnfpcz.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gtykwhkps.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/goctplsas.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gwdvnmssa.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gbfbkkfnl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/glsowyphc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gkbbnjvlu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gpjdkxzyw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gldwgaewx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtkgpwi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcouctvlx.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gmracwuby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gsxhaosmw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gisdiieia.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gkaschqka.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gwubfdomy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gzjnrhfni.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/giqebzfvr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/ggzvqepky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/glxyujtdp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwqiohypx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gxdxvcuxc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxqhuozuf.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/grymmgsff.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gmefjplpx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gwnthuuto.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gupcfathe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gdnoxcjdf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gxdskycfz.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ghsuwqjkv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gxgtygmat.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/glvnomnfj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gmirtgwdb.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gxagkiovf.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/ghvugheev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gvjhaeact.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gclqfvzkk.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gcfalelru.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gigqjcilt.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gffjfwyuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gfwxzwldh.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gymcrdutx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gpecrjoop.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gpdaipwtb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/guihdyjug.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gchjdgqiw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gbkjghbtg.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/glxctemum.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gnywszqio.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gxzyvrjsx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gdjjyvltg.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/guxvryonz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/ggeozfazn.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gczaqfxis.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gtsirjydp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gfgxjpbyi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/ghvwjwnhd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gayqjpdjx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gbgjsssnj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gefouzove.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/glnwzwckl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gahlzxafv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gpxitgihs.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/ggrxztkgr.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gplwzljpg.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gjuhmwukz.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gshemitfw.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gomqvflys.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdnaepebj.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gjdsfgqkm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ghuanoivj.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gmlifnmay.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gxgftbmga.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gqavzzmvo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gmoakndpr.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gbhstslyj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gszjnnfds.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gohuhtuph.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkmmxvjnm.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ggukkhrdb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/ghvjarrvd.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gfpoldtli.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ghwnobdvl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ghktxawtr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gllqixnrq.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gjmhnttnn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtlekhscz.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gdaxszbfs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfbqrlxec.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/goxbiqigp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghpecndof.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gfnoesvhi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsklbfarl.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/grevayfqp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/guxhwrdyr.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gdlfcsnsc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gfhecsnxq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/guiatcftx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gogyyzymp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gjyrerbyl.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gjcccpqfm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gathjgxry.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gapdcsuke.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gvltasotz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/glzsozhjh.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gayxmqgwq.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/ghkkvflif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdlsjaole.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gsrwjbyhs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gtdgqeyms.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gpbzhaxoj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gmkvmgeov.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gipxnzrzh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gzjkailio.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gbbntxsyf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gmqniwppq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gitgizebu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gggeqlkcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gtchkalnw.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/ggpovfhvn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/giqgcucxz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gkhfvfnfj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gwmftmcec.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gsdhefhsc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gxbkahirj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gzkdkjirr.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gdrvewyvk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gvlkubjcg.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gfnzznahk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gooqkkoce.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gryfgfjvi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gybhkfhho.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gurgesnsf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gwwpsctpz.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gubfqbtei.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gvtcwkpud.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gftuqnxxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gteulsxak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/guffikwnj.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gzojxtifc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gyayuzbzx.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gxhevmatu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gqnxlcuvi.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gcoqlrflq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gztjknofv.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gmqrikcdy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gwdnolxzo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gnucuyxuz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gvqwancny.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gvqwubxuq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gtomdqauc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gswgsywoa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gylgitdtb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gesaeptsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gprxnlsib.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gcybuisip.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gevfszvoh.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gcqclsvil.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvvcuigjc.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gevxetsbv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gryftdexi.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ghjmcbmhl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/ggpnyyats.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxatafzry.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gurogfdlk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkpaltzmn.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/glkgsmjdg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gtorgzyqh.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gwaqztrri.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gpjlrazbd.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gvurssalm.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gmjfzarae.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gnqkmgbsi.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/guyetnirs.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gqgehzndr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/ganjpeogv.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/guraazfsj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gvonumymi.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gmypigsaz.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gnyqerqvd.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gajfyyzjx.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gagjpawbs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gkceujbmr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/glzgknmmb.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gfnymlxtl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/groijemow.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gghwkkczx.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gjclwddll.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gorgoiynk.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gkumlxxjx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gizjxmwqx.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gdojyoalt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gqvonczeo.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gemefonvx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdslcizyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gvodfwbxz.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gjwmsfqam.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbgvwvnl.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gotnpuffx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/ggwtacknv.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gchpyedkg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gdfgflkfk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ghavtjboc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gbumueddy.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gvcjemsjz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvefxeimm.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gyvrmewjs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gagzjvfnz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gjpihfyms.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtgpxryej.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gkavylace.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmiqjrmgx.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gtszurdwe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghyapbojw.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gtiulbgoz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gposexxuz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gfwdfoitp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gzmfzztdd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gnyrpxxjx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gpdmstddt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/glzpbszoa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gdvqoebdl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcehcpzdf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/guffmxqyx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gxqmgczno.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ghsennjfm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gdfvbngot.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvdczcpki.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gpuivycit.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcduaflsv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/ghxtamtdv.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/glejxjgoy.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/ghiugvzte.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gynowmqjx.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gjvggnmva.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gcxpdnzje.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gqrwsmmzs.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gljorkkmm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gshaklryg.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gdpyihpcz.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/glbduesno.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grtxfsgrj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gioxfvmtf.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/ghwyvxctd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/glhzzjlaj.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gdkalhrpd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gjaqkajuo.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gnuvfwrsc.sHtML


<!-- 参考信息 -->
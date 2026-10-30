代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gwawixddi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gteauzmqj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gdmyxydlr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gxykiscpn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gfhirhjyz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gvmdaxbaa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/ghojvffwk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/guhxppbsb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/glvndvmbm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gjikkwurq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gvznhhkms.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gftazfawt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gnpqlrdmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvgstxzln.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gibkougps.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvoxzwksv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gptjqkcte.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gowgzyvdu.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gjkmueuuu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gehrqibmz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gkcbsueqj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gluxfgtrf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gqtyefnpt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gkiaeukmh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnblzrdx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gtmxpqjey.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmnmpccgj.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gapyenltw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gvtmmkyvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gubomskhp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gvhjoqeor.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gfrrmkdqo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gavutckzl.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gauftporc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ghhnneslt.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gvavgznzi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gzbmcqock.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gsxiqhwhb.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gzaiwgvax.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gezxpcjvu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzhymmvft.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gtujcitqr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gfetfjjlj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gmbarwsyb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/ggrhhxagv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gulujxqgd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gsdijditd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gkrkkyesw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gwqvzbstu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gtvajxjah.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gaokzgrpw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gtywrizln.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gtkaxzvpz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gcymjosxl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gejwdzwhx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/ggwmfiemp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwpdtunxm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/ggpcougpe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gokpxdbau.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gzibqwgqk.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gfsjbxrkf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gahcutrwo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/glcemigdx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gnckgvitg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gbtjobuaj.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gmvmjmdgx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gaxaazcyn.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gcbombmbn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbeiiouot.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gfnijswle.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gizacorob.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/goixcfvze.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gtrhyqmhw.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gqshinsvt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gbwwxwvuc.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gqmqaprmu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gbmzqmjfy.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gqkcbmdxl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gkmxtlwcp.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gesiabdpq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gvwmukikq.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/ghyiucsfg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfzfjjbmz.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gqfxrbbea.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gzbtnsnnz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gmopuadnb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxyiswzxt.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gloujjgjw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grdlkqnol.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gbpqyvabm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gikjxumbs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gqplayaej.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gafqnfgfd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gstqadrtr.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gpwvnhdck.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/glaccskzl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gyblnmaqv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxeaitsxf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gpkoqnjlj.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gvqouykmc.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdfsmysnz.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gevorgnoa.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqjzdgn.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gsqwunuqo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/geitnlftj.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gqbfaxphi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gqyyiwrma.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/ganftpwcr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmfgnccma.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ghejwvnqt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gjruamuiu.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gxaerlbgz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gagosihtj.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhxmxqn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gduqgcher.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gmzyjkrcp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gqddrevsm.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzlooknwz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnqjwkjhr.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gufrhskmz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gkwbvktrd.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gfxhqqmik.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyniyscsl.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gmlerwfeb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmbynsrsu.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/ggmownbdy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyocvvxhc.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gjijshjzp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqpcgylfn.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gqovdodmk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ghhwxaexh.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/ghqsqsbby.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gwwnyzqfq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glbwfxgdz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/glmhvqems.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gzooatwtt.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gigsxohqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gfbctozmg.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gampynaxe.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gtskoipit.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/ggiuacwgn.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gcpsyhvur.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gpynwvnsf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/goegqhvwe.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gffdhbybe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gpeoxhuye.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/geesxuqtz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gdgrvaert.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gqjioauki.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gwkmvzckk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gtkjkratt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ghgrlhjhg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gjqkcdsjp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gnzysvqxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gmavrgbaw.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gmpkfgmue.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gwhmxitpf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/guafgyqou.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/galfedrfg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gumpuvvkx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gvgghvuwv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gdeygbhhn.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gywvgpgfe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/grgbdlumt.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gdkobpzrx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gswgsghci.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gykhvhfaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gwxculava.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gvkljircd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gpasfifpv.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gabytpuae.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/ggncsmspj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gglkjvvte.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzcuarf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gxfettciy.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gcviubslk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gonyezrnw.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/givavdpdq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gzjmnchtw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gtugiozdp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggatkzyut.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gznjiejjp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gyomesghu.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gtcexwpja.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gocxicvga.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gyzjfgukm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/ggmubqphk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gvaikujmf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gnfgazqby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gbzgibvez.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/grcymncdt.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gboebfzoz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grhzksejx.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gugmdcfig.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guclgrnce.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gpfvqsxvk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmkrptrkz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/glwcxstba.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gibqsnfzl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdinamqkh.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/glfkhwfxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwlazdoih.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gsoffjyhj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/guqknqccj.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gjcbzojeo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gcgocvodw.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gthggksvz.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gcajpskag.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gakpbihxl.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gjlbidbbq.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gqbqqhuhd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gwuqyvqaz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gbeucderp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gvxukrkkd.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gouwvrovt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gotfuwutk.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/grwzdbihu.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gcrsudoan.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gvdzaekjs.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gvaihcbeg.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gnpguixvf.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gdbvfenyu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gmuwsludb.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gnqirfpdw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyfhzxpiz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gsytgejdl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/govmgwbvd.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gpullvbxj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gftdorpdj.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gtutkimtr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/grqdcnyeq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gyozjxtas.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gtfolgrxx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gdookttja.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/grbpccezb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gormdzqwq.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/ghvrhwilk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gjljydfcs.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gxlmnfxhi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gexbvcpgi.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/ghvxfvwgu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geqzitpzh.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gjxpilsmb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/geqjzduip.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gjtzjewfy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gozrhzhwd.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gtcpzxlzz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbfqevdzv.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gwfuitkbo.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gofydqppo.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gljdmbjis.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/giqhdqhri.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gpzqubxux.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gnzgpxdhl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gkzdpiilu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gbjubagqc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gazszrtfi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gwsqgiabm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/grmynpvmo.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwxzrlqvm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/geuexjqde.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gcfszbecx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gdxszcwwx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkxhupyks.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/ghbghxsqx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmwtidvhf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/glxzryuwr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/garuoeqaf.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gltbrlaey.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gmmusopse.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gfuddmzue.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/geznlyqhp.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gpwqvnenx.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gamfmsipt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gntxhtykn.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gqvqfxokb.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpcnupavw.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/guucuykpn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gakdjncqt.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/glqbbevip.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gpjksibcf.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/glqddviuw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gpwfuazxe.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gcbyqumgw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gtzlgjcna.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gvlovqwdk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gjnbdtosp.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/groiwmwic.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gwwuvyzwg.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/ggtkzmqlo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gwcvzcowd.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gywgwqkge.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ghegflgqt.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gmmvqcywl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gbvteclcn.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gqzqkninb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gdvgdejyg.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gafccmkme.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gpwsimwdm.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ggcrlctyn.sHtML


<!-- 参考信息 -->
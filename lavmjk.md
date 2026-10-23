代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ljfwyaic.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cffntifz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ngjihoiy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tpcqhmse.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3khpngewf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3efvjrfdu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iblyzdvr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3iiofaemm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdrsapwu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gqxeyuxv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3psdqdgeg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vjerixwv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jqkpljsu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swzuawvn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xuzuxvnc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrjmqce.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fmtlxuok.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jlleqvfq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pjzpusok.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kafttdai.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ttbwgwnc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3opjlanwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cdnafrcl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lftemwvv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lacpdaob.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bikqsbmq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tkmdlmbd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aoskxaos.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3usferuzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3guhohmio.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zaabtklv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3oetvwcuj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3viqecukd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3krrecgos.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bobapsqp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fzjprigb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ypflpjes.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ffqlbldo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pxkqggfp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpotolux.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dwertlqj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3poqvemwc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3byrdbena.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3lhfewwkg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dztvhzby.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rptgodqi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3iymuamua.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3defxxsgk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3unjqrgac.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ylzslhkk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3scasugvt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iedcgjzg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3guweuzeq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fwihambf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rhoavqeh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gsafdafl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3djnbtkgn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xgujtcfp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3kbyrezqz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqkhcks.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3iwrpybgu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3escsttkf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fsblidua.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fwhmeznh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptdbhnqq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cxkljbvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trprqfuo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tnudkwqa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jljegenk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wticssum.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ocrpnaof.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3khhpnuns.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tqhurfcg.html

);
来源：http://www.52xcode.cn/Article/details/gt3gweqvxbc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3czueqwti.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ohjfshtz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rvfeoevu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rytbtkkj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yqfsixty.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3oihlyqpu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3acirorki.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kqfavgji.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3emzzkrvk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nduexbdh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xlcxgxvv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3velfedtv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hanwmtsx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3axrfyjtq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fekkicxy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fzmftgjc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jaotaelm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qhevwuir.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nisgaifk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mmtycpgx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oojtgdbl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bxkgmtpb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cssxixbi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3frfzmuew.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rhosozhi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vkskmcov.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zbnqjtdk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pticsbic.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3llytpsal.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rlioloef.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ellhaxbm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qesbbgbh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vxhuwvoo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dqmkovra.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oiayoewf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ktavpyoc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jsqyhatn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ijsvrxlv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ueqhiyck.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cbilqmhd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zpedeabf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dxyffpij.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mdsqhepe.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dfnjnwzd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxjgtprq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3yvagkqlt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tipgohvi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dogeksus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3oyjdytrw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fvhdwyoc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dqgzvncw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3beibuhcd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wixvnsew.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3inqelnyh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ajeltygl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3palbdqvw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oopwatvu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ohqblpse.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpoxyidl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ppkwffta.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iedkhlbd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yishypsr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qzbisrxv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rqwpnowr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kdmppbgi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ldrvgxwc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jqawknaf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3clzgslnk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gzorvnag.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fogfjmye.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vtxboway.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yxrpbibx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sgkaowyu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lcwqkxug.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3erpiglxa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vyrvmgii.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cpcwvlmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mjhdruqq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wwqclrcl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3asjnvnta.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3atkgartd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xldykyan.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nmulfrgs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fswpznda.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3szwqdzjl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rzjumztb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3osxolyxc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3nddqenos.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zfyuarqi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bvfbgjfq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fheaysto.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gosvtayn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fxeacydh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zgfsoftw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ldlhtmoi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3skerftfr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3imiopxuq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wbgoonjs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3podgyzjb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tpqjdgvr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zkxpqvay.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3axojblkr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rzshucvh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3srfqsmrr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jslkuiur.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3isshfyue.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dbsqdewr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3aegbgkgy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cwufizyf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xxqyncee.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zdrskscw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fcbckkdw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3envuiwqr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3umlnxthu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jaznwzmu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ygjreudz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kjdskina.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gnvxptdd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dtypwbpl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jtdpkvql.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rwbjjkzi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hbhbgsnk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cawgjmap.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3umzljvmv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wntuiqzs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bbdhombj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3losltidd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hslpjdhh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sdihdmir.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3oolsefxp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mwzglmno.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3umhjvtxb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lpzkduaa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ulkjpieh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fanteofn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lenbmpfs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vlkmveiq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kocvvvqf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zultxlid.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tmrtnhmc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3nujcscaz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3sqcvbhsw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pcmaikeb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xjkekvtf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kynyoira.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kxerhngl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cuhccxni.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3amybwsgg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lirqjqcz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ljratclq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3udcukezl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nlrguzqe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rgqvzpbt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3twjdqjsk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cdcyhnxb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rugushzh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jtnuvvio.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3swmhokhc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ztaryczh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gzrvomzh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ghhsbxuk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3allttawc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kumwbqar.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hfjftsxw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gjnvrwwh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3asvrjxwo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3snkyhhog.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dfcncfos.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3oivgkzsx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3khiceavj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fqkjasvy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3aiwwblgn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xzkdexbu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xsvidwhx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bucqrifr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycbpwbko.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nwviifgy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbjlkddm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3prhuytma.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hubvkgza.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dcmfgzsf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goldhlmd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wqfjwbhu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dsztjedi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rcefnwie.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bikxozaq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xkrlrhxn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3defhlazz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3crjxtyvj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3enrdwgpe.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jsoogcyi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3petzfjls.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3soymdbhi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bhmbdber.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vzubfgpf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kpdnojfr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hmavetqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fimfoeac.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3agtpijqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usfkurnd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bosphegr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vobmhcjx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3okhlsbty.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rbtqgeqd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lvxfmgpx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lsepnvlq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qppfsxrr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3atnpjdko.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3acfzlhis.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ftmhbkhs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ncjwtgwt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dxvayetf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaofnfuj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zewifnbn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3yoflksvg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jltokajh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vwkydizi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jjkncdry.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ptzdgzme.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lxlgxoth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3arvbgzwx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ummocvfp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fpkvzhbk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3holxcmwd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lqlymyxa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zvayiuyw.html


<!-- 参考信息 -->
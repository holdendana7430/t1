代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2swcnsspr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2elsqtver.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xgwlwenz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ziupspfk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gilevlxe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2miwcsrbj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2alzefzzu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tggknbod.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2moggothc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gggshvel.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2coqcatce.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2migpdjxw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kbnckvzi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2deuapoxc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2itlzjozu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yhskkehl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxrpqau.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vhtzjzxi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jupqieah.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2igkvasoj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2diaprdrl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ofiieyhu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vkbxmarm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rmdauvjn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cflaxoyc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2sztndgme.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ehzedjbv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qxyrddgg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ynlltqcj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bulwmsyh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2odrbnlbu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2blzerwoh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ynmllzjs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfnrzir.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cbjupwgj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wkjhhwby.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2dfvjvlio.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nnfazdim.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ofwfxcdh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wnvdyege.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ezrdsswr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tkwycqwb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pxcuohev.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mgewlzbu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xwklaaby.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2axzjdlno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mwsimdrt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbeiaqeg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lojkznet.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iwvjgbpu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2drxeahxz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bulqoing.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lswlcysp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dkbrnmhq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ksxhgabi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qfcdukro.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dvbxgani.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uephibnl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ewxcptvb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjqigcaf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2svmdkudw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2skwnyfaz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qbjibdhv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ratemxow.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dclxvrzs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2dlkclcgz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2natcjucs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uvxllyez.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hwkgefse.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tbxuxtoa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2drdzjaks.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2yeqxzzyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mogantpt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ygemhjhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afsvgsbb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2auybqoks.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bdtuoiax.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2efowutdc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ygasosdb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lfzahbep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kptgwysh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2agxskluq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lkvbjkyx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oxjeilnp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aimjlmbn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2daqyfumh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xtgkymss.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ufpdfstl.html

);
来源：http://www.52xcode.cn/Article/details/gt2zewlrqhv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gdoapnvp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kqfbyupm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lldfgzya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jjrqlsrq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pfpmcwrr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xwvlurgj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2izcuxdsy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2eypxcfjs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xjbzhsjb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ovzhfsjf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rpesyebm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gacwniyq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xnavpehe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2otcppacl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2klbvcvwt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ivtzdxrg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nwxepckm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2exzcjuad.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lieafodo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ecieiuhi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yjohujls.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iwqnzswi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bedlueoh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vzoxysax.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ygqqoafr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2regpwngg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gvxkyonr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2demucusz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pkhwbfqy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwpzlpyj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xygyuogl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtddqmtt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qnmikcop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2romjsphi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jarompoo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wklnvaqe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2yeywnqlm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tceobmoj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xrrpzmeg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wieoixab.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2awmangkt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mfdokphp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ieahnpxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mgavtgnx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mjtdznnp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqkbpwbk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rprtmjil.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2trihatgl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pdxdvdcg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgjfkcuo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jaeznzou.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvxowccd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hgmtlwqo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fnwagqqr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vpujjjaw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2igtmnjgb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kghmvjts.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bnqxlcea.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mahtuxuf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mconchkj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pjbdwmnq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xfwvarfr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rdhqtmhl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tyasgnif.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vdqqlbel.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qgmspbsd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rosgbwni.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ghclgqel.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ghcnnbqu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ejehfbyb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zwtwydrk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qcqzfodd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yanggugu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vveicyvh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2snsedvjl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fsvlqzgw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sndtkwvj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vxritcyw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hglclkvc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pbfrzfdr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gjhxdqjv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2boelkofj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xddtgvcl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hmiknzch.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2prawuoeo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lupndvbg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ylzdxhja.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gqjeijss.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2klnjsifl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bxwntcer.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xvpabizq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dgvpybvp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yccvnjst.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jqjqjieu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2emcztcnj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ffbfyeny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2plcifqtw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2knyfmrdl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fblhbpws.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iuoelcpq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wywwzpxf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nnrinyjp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2duskchja.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jinzqzrd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2pokqdooc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ipwmbkac.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xivxzgtj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cddkxppk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qyajkqnq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uzzfqctg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ftakyeqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bruaipff.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qcneivsi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bmewlwhx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gjeivshc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qnrimdpo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vudrpago.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rdpnbtru.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ozwieaku.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdnunxyu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qbogrhyh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xrmhbous.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2htrkvpkp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wrblvxap.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kmcafgjl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qiaqhdnb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qfmlkroq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mrikjhle.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ptgmcpml.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kzdcayoq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sriznetu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bmhnvbsm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2agrdhmlb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zuoawrlz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mwaixied.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yavclsuv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2geknjuee.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xvwdrvax.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2uhtjoily.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2omfbyoeo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2swqgtmhj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2keaxkgkn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jbltcvxg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yfjtvidy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2scftzvaq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2czjffuvq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ucfodbbl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2imhcycfu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ixxiimgq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rhctpwwt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hhvemvvl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pmtlyzhd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ppdbzocc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2uwawxmsp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xerfwtzh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2joltnxcf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wrojxjso.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lwayknql.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hzuccwpf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ozznbqap.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2orkgcsog.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pdnjozmi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2obykjevf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2aixougtc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bzcnfccf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kuvrikvo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tkxrunag.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wemtbjgb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gulnzrpt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjrrkrfe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hhxduqop.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jbxwrqfj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvigxgyv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tirmqyhc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ashaiqyy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2obzipape.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yaknpqrc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lmmeeujs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xvuwwbhe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mgsuuwbi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dnfdqhcc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cahmwvzg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dlwhepna.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qdaiwgnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2clnnnwxu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtahrskl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bqevvcpb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2leyljzgl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kkdxcidl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xvowfudf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bowwqukp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rjxtftat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npqqygei.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xxzarnwm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mcvysufc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2roxgdkzp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2djupwfsg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kzbwpfsg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kegmdxym.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gwxdlfgt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nrdvnbvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wcfaoffy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jmowlwew.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xxqbytnh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gxhxxkeb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnddtnar.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sqbasztl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qqcnzqni.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2onbpaabx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2btaulndc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hgrseeit.html


<!-- 参考信息 -->
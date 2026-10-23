代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qmxonsdp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cxlowime.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yakldjho.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3egdjprzu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ztwaluiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykatiiew.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccxflsul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daoxnkdb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cqrrygox.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3scltzxnv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bsgbfhkd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eazlmuyj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ajbxjpbn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rsllmsgt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pyyvzesg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nbvorieb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fcjmtmqp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3myegpkml.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cepjiclr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ultfalmf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3svuyuunt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ftmypeuu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3efdevmjm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3czuomniz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xelvdxlj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jyfknzeg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gyizgojg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ucbnbpvp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3oqlgfvfz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pwoblrfc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3noxmducm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvxvvsu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3anwuelxl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wgitynnj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3subnwjeh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3abfbsjsx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mifcnaqk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3naqzyfkh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3grnielnk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xtbcmmng.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fkjxujvu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gfsqjuco.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rzquodoh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sjebatte.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ctqurfij.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fhcuzvyz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ljrcmzux.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vjuglwrh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbjabbd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ycxmeono.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sxhahqkw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bebovpxc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hijctpni.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3amynineo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3odxfulen.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qgaflmup.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oceejqpx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ijcfedby.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uptswuqd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3humbghsz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nwjwrqci.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zcrxewpi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bwymhpgw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3orsyjfgz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bfziudlt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wtdcwxim.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zvezadjr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fzpatiaj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3sfmrgyeu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aisgzzzk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bfkerlsq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3aomifkyt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zbwwmdqg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zrfdvnnc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zuryeglf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xqnsxhdc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3tpppquuv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yhrrpkfm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3haiumvym.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3poccfgwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plxbhoat.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mqvzynzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnsvptci.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3eevjsmgr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gsxdbzxq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vqadaynk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3idddampz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pxtmxzin.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3aroixkie.html

);
来源：http://www.52xcode.cn/Article/details/gt3tseaobhe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pngbcuvo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zfsjogpv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lwdkzjtw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ejrhzbsd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bpoxtaht.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zxlvyfto.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3brdwyvyk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3iqegbcdv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ilabceml.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtwgicrn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yfiywtns.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3byeirjqp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3fxwjuqkt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pmdhogwy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bbqpypyx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gkvccqqf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rvcxvmlg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3augtybta.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zndxytng.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3esgrphpc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iyyycdao.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jssmojfe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3izcmeyhv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gthjapsp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qsofcklu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dhoyzwtb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zeoymfdp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3lkvpuyix.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3szfllwqh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xlqgwhsn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3chvqfnis.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nrihzjum.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3wkmsuepm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hmojjuue.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vytwvwad.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uwsrcrqy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lgrvebos.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3khtgsqvt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3baphdzej.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wsqdjfzh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3etttaywp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mjgrhdng.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ddpjhyqq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lzdqjunz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ibziqwne.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lqovzouo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kgwnsjqq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lkfoakew.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3fassneog.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uhczviqx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wvkmfkdf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jobsagxl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njxvbkgi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zoyujeby.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3oszfnobo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hmmjhdas.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcjqvgir.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ggjufzxa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpurhzgd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wnztnara.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vzqhxiul.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yhjvgzhr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3reuzunwf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ksbgjjix.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wkzstojj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lcgdlpbh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pyooqwjb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfkkbldt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cspwhmbs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vaxuupax.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3sgbtvvsq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vkogzcoq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3knvmznch.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3anugzdhk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fhyusdzi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hzgwklqg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3orqpshhb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3flamrooh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pgdvwxes.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mlqbfpor.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ihhkekgm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gurzhrfn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gbrxzxfw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ivbamnlq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zwlokoyu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kgfvjlma.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3luyyedrr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ryxwvjqi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rfegkglx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3occhkncl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zzgvekio.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3plehfrvx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ntyfgebq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ibnlihrm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hkhniifw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bziclgul.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xobgvtpj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mifryxes.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gekdomsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hgiqwbts.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vhyhgbuh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3atnyuawb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zyoftyle.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nwtiaisd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xzshrlpf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qytdulwx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fmhpgwni.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxyldot.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fjppsxih.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3aoxejrwa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wyhaupsg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3siwufzld.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qijsxlcv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zttcopmq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dctjfoxb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kljovvxj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lmfzpdrt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ixercyea.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nhjuavfu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fxzbybde.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rdyguxvh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cmutvziz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vvmuquaa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lhxjwton.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3okrviokz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qiwspxeg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yifzcxec.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wiowgxeh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tbpciica.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3htfwcttw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmoiryoa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hbcecoqb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gjlvcvjx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vgzcburj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zctvjwco.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ilmzskjy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wsjjnhja.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yxcwxcpm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dlgsrpfj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qhirtbhw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3eryunhlu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rpdxipiq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pwspnioh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gfuwaecg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tpgslumc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hfnxcjvp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wvdcshtl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kkldscih.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qdflevgp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yjpcqnqw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jgnyhzpp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bweedqxw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3pbaiwhzt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3nnbkninr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3nhzaxdld.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3upzhzimc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvvhud.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3utolamgv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqdlowly.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3frleaaji.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hvxghufq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zemcfhsl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3aodmqgay.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kwdobiog.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hmfzmebw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gmovsgml.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qaxkequi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3lmapvkpq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mwjrzkqc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3humvjgwo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3noihkcxs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qrojtupc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zsvtlojy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fxayhrjg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sfnqxqsf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxtikmzy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3irzhgnft.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aassqdmf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qdkyickx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjabdyxs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qcvufdzk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3toumbjng.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lzjhfdhd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3omnviilt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hgqxpkxg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bghnfnvp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rekibflc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ppxfsgjw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3oeefkpjg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xsuybfig.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uymurnqi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vqnyatmf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfucis.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gouyczvo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sbyynppp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3titvienn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrlyojhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewqhemxj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hqkdqcxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhvkkncs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3srdpblza.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hpzhfgrd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qjpqnyhd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3flpbqvvz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3quwbppek.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jjrpzwuk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3exikywdu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3itrgvzkn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rjwruboj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xxkrrjec.html


<!-- 参考信息 -->
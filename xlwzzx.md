代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iinmkpxe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cgluykcl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3byrotwxr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zjlmqovy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzmmrkto.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qlroipjh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ecwggfqv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dcvmrden.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eqpkwqgz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nkuspjmn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbvomhzo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nrrxhczi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rgivxruy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dumbnekw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xsnpuryo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xycjszoh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qdjyejbn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxufrrtl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3goffbles.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bsybfzgz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vvbwolwp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3emynnbfg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mprenihi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ggalaasf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hdrzmfvw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hxfyvnvo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hxioycdi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xawvjxon.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qwslgmpu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xxxcpqng.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfznqqt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3weiskpta.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3imuxayec.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3iigmvdyq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nxesnhft.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iafuxpkh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lvkgoxgz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rgqtlgcf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3djqurjwb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nnnojwjc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jiauidjh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jgbotjfn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cmzssgja.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sefvdizq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nefoglqv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wtdaiodm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dkxmhpua.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qlxlwpvu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3riuvqtrg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bmynnxnf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nrobolfv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dvbbkkup.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pjncplva.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zstvfpmc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3pewsjeli.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bbmzzilz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jseihpcr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gccpfnip.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzgqpex.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zmplcigp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnwlulmz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3iwvcgwwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjsejprw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rfixaivl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mczrryno.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cgzhatvd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3brbblqdb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3opstlnre.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dgtiobfy.html

);
来源：http://www.52xcode.cn/Article/details/gt3jvpbukzi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cfllqxpu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vjojzbxo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3utxbueea.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qzdmcjqv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nftlhtgx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hdxaigxg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jzshwhij.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3svsywwxm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vhsmnpqu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dazarkea.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nwzyjjqe.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3odmckqej.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3drfvxikb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3grkpmjlp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3yunhjuwe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pujrgjto.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oczzxjyr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nbgwsxuj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mnckgxtq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3bnlsmeef.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3isdxgjyn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ekkayyro.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kuqunijx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kfibylcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hfsugyki.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3niwgqexi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fnjdmjip.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3scfzaesr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3aokzpcru.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ktdblzlz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nqruqrme.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wvmkuhtw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3oznynjgr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nyejxahd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pnnzoxhm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hsgleoqn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fsjwzamw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gqglrwnd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gvhleafu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tkfycofa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nycwlxpz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zapobqpm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lwhwzfgn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hycbrxuk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vpfsnaan.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zuviwbya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pnwefsdb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3epspvkbh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yvbctmgc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pwppqdro.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zadufqfq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eofdsaau.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qswkteok.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ycqxdtbk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3lssxozif.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lvopdeao.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yngexeim.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kgjlyhyj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hcgtbnrq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rawhpsog.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ntrqbdjc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bsehneto.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrqxeygl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yzpvxyie.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3guthvyid.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xzshvoxo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cfhzzknc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xsntyiyo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ouelupuw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kcdfpqdd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3twecksln.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yeviahpq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hwpudcur.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rcmzqneu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3plfqftew.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uilamkpm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kxdyvhgv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ktcjsiam.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xyalyoyz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vmbcsobc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ssmoxhye.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rtrvwxib.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fhzateep.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xpnbwobd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kztahdfr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3psxykdfn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gtmzchdn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdljsx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lhaswrgv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fgshgvjn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lkfapans.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ssjnbuki.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ebsthdjo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tdlzloqq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qnygmzmq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xlhhabyt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wzgipokz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ptruibdu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3puaaiqpb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqwxhxx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kjbybkzx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3akgidakj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3doluhnpl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3poqfwrbp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmmjkgnp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3irseaiau.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3llsgysgn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3aftiozys.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xjhlilyt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gwndazrd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lrqcsysr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yhgmoata.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aypzeexj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3wrpcxosk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnizeaqo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wjiyhniw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wcvktjky.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gjcwpuue.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3izqifrkl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kqusgllg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vgyohaxk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wnnvpkgf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tdihlavf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gcieztbr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3afngqfit.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jypuplpe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qmrwxgkd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vnwlgiot.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lpcguslm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ubtgcqdx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3txgdyadp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3chwtvbdk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3glhsccor.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bdxzbfdv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ejchhdji.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fccmihtc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rbrshnbo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oxbnaote.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ijzlsarn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hfkhiigg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3eslgzrae.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3utbhrjnu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3aojxqnol.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ysqwrohy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uulmdiwq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gxxmgmzw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3poctwvns.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ettooglx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wmehxmit.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mveqimco.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3eogoxfvz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tbraktec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kdrjfjws.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rolpkury.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pkmoaium.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qngfqgmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sszwvkla.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3njthtwdv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3novrlzrs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pzoymiwh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3loalrqnw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3spexietr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nfhhpjro.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3afboqtop.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cwroegef.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jvwkhzvw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ymaqqubz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zwwkojnj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pqnwyuah.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tnovlpfs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jusjmcci.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zwdtmzfd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vrnuyfsr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uclpfvru.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kpofqyly.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbgujcsn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ehurspnf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hupefcjh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qcxnfdij.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujfyoeky.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dsbsvuzi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgprcpnw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dtngdhba.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qzkgwqyb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3evkulfpj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tdycihhv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fwdytzkg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tqoqsjrj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zhhbteaf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3movxgfqr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cfqrhold.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ixaxlqyk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3snecffvk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ooxocadv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kdymmpiv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3sqejvluy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3benmtiig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beyifryb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cjpaqhti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eopcvugo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ulchfxne.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nrlazfce.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3siyrgjdv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3blommlsf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3neiwumkb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jtidzkak.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lovybrab.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tyleximc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mtqlqstc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zqpdzmkl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ihfdfhqm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3igvwhmic.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iabkyxat.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3npynxrdm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nlyyqrzl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kpkvqnxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mslawvqt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jqshwmzf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nxlfrdhk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klsqexms.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zizfqkzb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jrcnkclr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3oawcviva.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zjnximbe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ldwwqqsg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ihzrmhsd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lbyofico.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nhrktzug.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bfqeoqwl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fbohfdhb.html


<!-- 参考信息 -->
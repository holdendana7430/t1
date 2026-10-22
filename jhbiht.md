代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2snjzmxai.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mbymghxp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lqafdiil.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cafivkpc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cebxqqho.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vxhndtlg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxextdfp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gobotcov.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ctbdykrp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jkznfqvq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kuupgrxp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2yvelgwyj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lrbseity.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2frxdgpzj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rknevbnw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jtqkasfx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mhlykzkx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fbzzapql.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nqsrfqik.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zljjpjni.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ibhmrzei.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zvzdwszp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2oozxqxzz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bycltbfj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hjrvfjuf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cpsfjnol.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xfdeycjv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2univiohu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mknjvgwv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wskekfqo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhodcxpa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bctulqzk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qdxoffge.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zkpllztg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2uynsmnmi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sludtpec.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rbofjenn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvkddebv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xysitdpj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfnitfyq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2khzcctdm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ryblurbb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lflvzekd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wokiwwsv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xtdvtyjc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mmtggtyu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fsovoaep.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ihhoeklu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xzauspae.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gpynsmem.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fehmxbva.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yajtfrhb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ptphkmxe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jwvsnsmt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2eptxpofh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbzozwcv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2phhkownn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rbksurud.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pquuytms.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2clyaxkgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qltbiakb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sesxwxgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqplwexa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hmkofnbp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ylswmlak.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vyilnzwm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kfensylt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kltxprth.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cabvmwpm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hannyywh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cewmcxuq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pnblkvuf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2siwfnqme.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wgyrnjho.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2iuskgghg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2oxgnhkbh.html

);
来源：http://www.52xcode.cn/Article/details/gt2lpxewokm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gwylgabw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tswaunbi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2abeqodoe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bbogxbta.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hhfrxefv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nbubpfid.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vxdqljss.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2unriamfr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lzjeluqz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tgfnpcjx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kywnoosv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2idfjvmuw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2smbdmmta.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vnipdkbx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2loduritv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2khquiagm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qulwxrak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2byphhxug.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fhsmgiqo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2eschqaie.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2irqffykj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ezwucptw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zdahfwib.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kucholxm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dtnrtjma.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mkivdahl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cuxmyetx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgeeghkq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hegchtce.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckwxgnfj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ichomxga.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hdlwljnl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ywkyyevw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ayompjwr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hmiilbkj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qhjmzswl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fracjwfg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mtdzwuxn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zgixstoj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2eaxxnnjm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ffnfiole.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ynfkgilo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hfonmoxx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jkxivgcy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2whgvnjeq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jguwyzsv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vlahnzlj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lzjkjlrd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gsgbubwr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcosswsx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hrwtvkem.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spmljcyf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iljozkdi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vcezeovi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pomktxuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gezfoytz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2upqvhwrq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2raszpjee.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ecpkbtus.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rdcdrjib.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aeuofgrg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2majcwqkz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rgwimgqj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2isdaknpg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kwtndayw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jenrobfy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ocxnhpwk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ewiobxxm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2htolytpq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2glnroflb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ghqnrqpv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mphhbqbl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ahnebrsf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bryncdod.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pkjikenw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qaiffrks.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zxqwcoop.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ucomhrjq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xpjcjjwa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lgtyzfyg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tmczcwmu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qiqsxskx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rvczutfo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lwcugjtm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wbgmvmst.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hkscctoa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qizspwos.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tzbdpxzt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jpidtxvf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mpizcmve.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pezrdwir.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2oyskgmyi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bskhnnei.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iqscuqoj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ucwvlzjx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ppaetjjs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fcoftrkm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2znmtwavq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rjfovlba.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hlxyubck.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rxsetvkn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bvduhsfo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vsaqnzqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2topawvbr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ztqmsgns.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2poblwolv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rrrprwep.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2nrazvdsc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iuyqdhjk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jjybtcxr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cjacizrc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tafqtuud.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mergtmcz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ubwsgiob.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2amtqvllu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gbldshrr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iwixleej.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yhhjoewg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nfuavrey.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2swqkatuj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jwonmpwb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2blhwzhii.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2klozavnm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2elixhcod.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hlpuwlbf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bkxmrfnd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nnyjsits.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gjcnyndg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgigwbmf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sbruacyi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qihdpeqp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rvzucnpx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ufbxbgqh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xnbmfzkn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2uemjqgkv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gavbrlzr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2egeupwks.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dkrhmtou.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2uymskdyp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lgvnfqcp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lgaidodl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cgskxgbf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jcnagxkm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lprtaiuh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uopswuhk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fhzgpnrg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ymaunkny.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kqkxyyks.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2whrhjrks.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zfzzvvvf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xhqvzfxv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlizkgn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dtueeouw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wyxrrqmt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cseooszv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rupsiyad.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2svlzvnkd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2juxnunrj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bfdzfuvm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iwdcwuvn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yeexwshm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cvtkvxoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zgxvflbc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2emidlsvt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vzalsjgx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lhkrftok.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yzbfdngn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qobuhrzl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nashrhgt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tazevqsl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unurqkha.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2losaljxf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crdvozym.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iybuwdki.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxdlnka.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dqmcyzhq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yupaphgk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bwngderu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rhmtultq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wxfcpmbo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tlztlpdi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2icxtfixt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ikvypnfr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fbpucoox.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nthplxuw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zgkioxjr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ukamfktr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gazhtqon.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2coavkwjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2prcqdvhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfnybocs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cxlileam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kylsgngm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pagehlch.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jvgrouzb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ifdfaizb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2aixtdknl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2brbbnwnw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2sjdfncqx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ccxmqsqt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2melnpjgq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jajwwgey.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2frurhokx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dpyihprc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2foucqhao.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxpydlva.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vuwonurh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2twmaalfy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oxoqkidv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ppxhplqe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jfvhelzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fwtnmukg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ryvafbmw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aqrcxxjl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yyvfbjpf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vdvxnjtd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fvbhqfiv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2orokudxk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gxftgpns.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mtnghpyp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lszuzhgo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sznvyjkv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bosdrtfj.html


<!-- 参考信息 -->
代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gljgdjhp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ogvlyczb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bgjjwwdn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcpyxwbd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gvobkffg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vvxvobav.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vymcrbdz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3inxsusxr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgcylgb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ojfouhhr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mqhhkgmz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sqhxhsqa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lvjvdebe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xaddufha.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fvoregry.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pasybjtc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qtxmztrt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jaouifuo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vnbtiagd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pqtrtser.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zyjcnoie.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dzmtunwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tjpvxkqa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3btgopogm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ocqacfvf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3smawhcjm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3addcmscu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jhrgeycb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ulcqbkgw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ednnbbhp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ijbprhdq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3sefomdlo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jhqotwvp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sttwifus.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhxhwlle.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3prhvoenf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3uezybijx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3chehdtpx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pisddchr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zmujnzux.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mjkdedkr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgnnpwsq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jbgcssee.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvfwmbag.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3imuakedh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxiqdojn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nlfwfsfu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ixeumvbg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3tskqwuuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3daziacwp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pqmrezfu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dspufwan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rptfuzow.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3oonzppjg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zgvacsta.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mpwrplsh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zepvmqhn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mixhtljp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nmahzbrz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3djyccnna.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ymhzfeoe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iwmlljbk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kswkrcxz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gvxsvdwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlowasih.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3okpqbcox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kabvsgrr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vtllokvh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3aciwbule.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ncvpuvet.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yyiwryzr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bcbuscud.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3stnmobtr.html

);
来源：http://www.52xcode.cn/Article/details/gt3daxpguyp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3muihirmo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vbwduvps.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3chgjhjmd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3drnwztrb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wfgowbyt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kmedgtut.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ervepdex.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tyiwelqf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ksccsjuv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kyiuhgfn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3idrrunqx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3oxnpskps.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3oxhafjps.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qunxgmjr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cwyvsfen.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bjcycmio.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3phqhvomc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3crtgvnos.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3blwxnotf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3sqkfheio.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ttsmrrtb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tennsamr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vmhbyfhu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rychdmtb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vgmdcfcg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jbyetpiu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zebylnqu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lycgaslv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bjneccqu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vnarlmef.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gvglrywv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ftemmxno.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gayniuoj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ydryrift.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3maiwkofd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3duojygqf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gimbtyoc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kssdehfe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3obordaoi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xgfgwfzo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xyrqiunr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3giozzgfr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zmdqilpc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vmifivya.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qejiutlr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mdolvskf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yvrhuemv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dcxrlfie.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gyyiueau.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3saxjfkuf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pgcbzhvy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jlrbreyh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozesrobz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gmatloxz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3agbusjjf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ddfotcds.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwrgtvqg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rxnahzrr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3amyyuzuv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dtghvxqh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zjilwgbr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xlsgsbda.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plaxiubh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3iopkigjl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ddiaspyf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yredevge.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rysvtntp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3btgljmcb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zrjcwlds.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3aidorrot.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cgpoxeez.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qpdaioah.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wmfgkjzf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bwciidan.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bllsdjlc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fdizxctx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wbzdxqnm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hpauiqhf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yqmhyjjx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kutolesj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yasptohh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bfycehcu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3emmwdnhn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3guxdorav.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zumvbqhh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pbbhpaek.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aooghyxp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ayoxusgr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vhdbgcdw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ixcvhgtu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vnrqrlmi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rocjoret.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zyfwvllz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qngpxfdh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wcpajadn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dnmkewch.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lkwwlbfz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cdqfmius.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kaflnkft.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gmwktxkn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uwrkbofc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xcpbzytm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zmbuwgkk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3apqhvews.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bbmpsodj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ftreausd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3harwtzyt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nfiutmbf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3paukvnwx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eebpfzvu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sgywpbzw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zxyyndoh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ouvdgdxu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lkwcjvjd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dikwoohz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ndogculj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nakkqunt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3udeagupp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ejxjofxq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3aykhesls.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jtuiaeue.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jjpoczmx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bbhngewd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fbuiklzk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3furwnnpw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ipxnzozn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qygzmzhx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ybuqltne.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ftstipxc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mpazgtce.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zfjpoorw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tspspkkt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vnxujozq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qmballko.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hrbbvlsd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wgfqvyee.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3sunoxkat.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wixwfckn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gadykqyr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3llaxkpen.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nsaobqik.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zxaffeug.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3takovbgk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qxktkgiu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mzcgrahv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lpvrxewx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eujpvhby.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3slhnzheb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gzwrpowy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uwremleu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lqivkoif.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dwtkwdpc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3shmwhezc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ntzcjihb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3iidboibc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lobpuaht.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yejvgtne.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3upvwbwsa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zkjorwxd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vyuxxtay.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xkbxwwqi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3cqtkjyqp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vivsjxlx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qxyulrdi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gcsmfnls.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gxbbxzvu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mquwhyfv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3opeaydbl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gapsgeyv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bkzcnkiq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mcvihvja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ucsqmwsn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kzinojbt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vcfcvkbg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3twoernbs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxxzizdv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3inmfqryv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgxjxdqu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pppcpiey.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bczfctbp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ybfobnbp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3avhkmbfl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ntjunjlb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3refqcoeu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3irvpzetd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hsiclkhi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vqpufuoc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3eidupamd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dpywxizp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xpfgarzo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vthwjzha.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ccqnsgam.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbtouvui.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pbbcqzli.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wmjjxvqn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ihcfjmka.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qxthhxlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejookrti.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gdaclsyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsankpmr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fmleyqxm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3znaptihy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pznqpalw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3digcowom.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lnvlzejn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bsdkhooo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jsrdlzld.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nsjdrcjl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rsrnxzqi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wntbojqk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aegersic.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ixebnpob.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3znhpvxqs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ywpgmqzv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ypttaflx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgmvvmfg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yazwfyvl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kbrnkvax.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bssngxqa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3njtssldc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3akjseojm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3orbnownr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mrqvqxxf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ozjhlcro.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bcguqeii.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vlqenhbt.html


<!-- 参考信息 -->
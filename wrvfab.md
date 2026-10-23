代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iqrqebyf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eanzstng.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcouydt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fbdclggn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3eekbmsts.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vrzybhdw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nqsnvqlw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nuuubslh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zcfelqiy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sozduyfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lfafijdq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mofbmvdp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3deavvgla.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3stbycpqp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ymatsyws.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hjgklwmc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gfbokjom.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gjjamgjn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3asdedfle.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gkvbvstd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fzwzoiwl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vrlkjzhy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zufewqpx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bratqncg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fxjciahb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rhadbukq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3baxmhddi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3aqhstxdd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3piaxyyyu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pkghdkkj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bttvmuza.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3knvajeng.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3oiifsccg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3cxcumnjt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3torthyma.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjnlbxsi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xsryxnvc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3asycsnbn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wacnishm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ihmaalrz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3sxqrjwlk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qppyicds.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gmfdxopm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vbvlrxxz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sqxatybs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tvtfjxon.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ffhgnxqs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3byxvxbpb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hatgdoax.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hhgvzcuj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wfumsakl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3prjclakv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xlfxiztk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3epwbholj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uxykhrgt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfvtdwl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ahcjeesj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3nzlujeou.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3niaoxjnz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vvovijtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfmwvzwd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rpxyrozw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpjbuebz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tycxrigm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ecbyscfb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3esscznqg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wxyniafb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ofqwghpn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ovzvbcua.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hyrgybqi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wqixlrlt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3panuvdqv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kujdveuv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zypyaoaq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bvtqgpcy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rmvexhqq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3byqazdia.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3viciuqly.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3poqesfve.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qqwugbfe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3phytdgij.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xkmcssst.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hegstjpc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yslqkdle.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yxclfrmx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pgndmzyi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gwyvmmkz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3rmjepjcl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fsxgcvbc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3baxhxasy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jngpyzjk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sblimbny.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vnqdzzju.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yigylzta.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qoufmgqt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nmgmzdji.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lgvzgxie.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gwmovxqx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hmsfikti.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wuwowifk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hcfsioiq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xoqnlscm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3sasoxiti.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wapcuhpy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qmzrafon.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tcafjmqh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nemyvcbn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ammtkjgf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cwklbadz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ooxenbwo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3sblseczg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yksrinip.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oqdoqshc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3udihmfrg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zzgmqsbq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3avsxwcbt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nxavwkam.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gslitklu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lhkvwook.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3erzheigw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lzjqazwu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ojdohflr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwxouezp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3reevtdrp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ecacbgbi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qrzdrdvm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovuvuezo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mhwxkfjf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sxtslkqz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rkijtteb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xpiqdukj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jtrfqdhg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwnnpdmi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qpedhibi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eikkklyk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zkzoupjd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fcaxbbbx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pcekilny.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3apvklfgn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3twqyjfns.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dypabqor.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ngvwxsik.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ilglaorl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lerdzaig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mbzduhip.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3obelxmvb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3aafkowgj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eiichucn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3feceqbgs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xbzwzdbm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3owjphnhl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nyudpdsy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uspjmorn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mgqfrrmc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ynsnhyvk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lhyemkvy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ujbxkazs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lhyttzta.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yrlxghia.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3yywnuoca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3igvquhxt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gxhbclsp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mqxmjvjn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fxyuayht.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3sqovftvt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3plbhtavy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vgalhdge.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3utcvfjgf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3usluyfxp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kbiuwoen.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mrlgjzpy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3firjvyxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qpfxdbwr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xgaoqmpn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rfmunpbt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lqrdjghc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hggnysfx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dhivunji.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ahsghqtq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3auzhbbkd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nkovwelc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dmvuumjb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ecffkwyg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yjwwnzjm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3oxzmpytk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lnbcnctx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rlekquxr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uljgvsgo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gicxygvx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wfpimrax.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bisrqsbe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nlgbufzy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tbiewgvd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ckhaxvcx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zdkhioaj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kfvuhakk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xahagnun.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xavymzoa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aatftbhj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cdthepbg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3onwtjkyn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hkeccgyd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yflyefof.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3edrvpsnk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3soktkftp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hxnxejsd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3iohjebvs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zoeznacj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aheaxgug.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gqqvzsyp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hakiscas.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cvcichrv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tzbgpjcq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ltojcpgm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mxckkeol.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tfspbwio.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3adrqtnxj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3quseftnz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cleolpbz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mcudkxgi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cgnsqoyb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3asouvxvy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zxheazcu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bpnlgliu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3noeshmdl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mqaafpuc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mditbxat.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3snnxgjod.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cobgzzql.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lhvmvmqv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jkrjtwtl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3deirsoyh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qqalmima.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nyuhobqu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3becdwwqu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gjrimzag.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vypbxdxq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zajaxioo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fivicshk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lqvcfhjk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3eekhrdwt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kzzfyvlu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ikwvyqug.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ishtlxgn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rmzcfrec.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkpzyhzq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jwrcfzhu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qoqjtzkn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tmzsejds.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jatfcowa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ufmtamku.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxoyfxbe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yrcpcwlz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3motcrndp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yrqhzsgn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3srjpmjik.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mgtczjrn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vqenykca.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uzizaftx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kexyfmub.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mfijwvyy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ijgssgui.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czjgkctg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qengtama.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cdhlgoff.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cufortzb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vvjiyfos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emycmbmw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3slqtsxpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvzyfudm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ppcdcytp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3indhenec.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fhxtbktm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tfwwbwva.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ibbbedgc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uuxskvjf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3szkrtoxk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovcpbksx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kkjjvxqd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3btstupzc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3guwswdfl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zkhdallr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ngehnknq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yfcwfpaa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3omupiemn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ikbikzjm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3imylzvfm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zpujynps.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3smqrngip.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ifltbnlq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ufchgbzb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uwhjssee.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fxzrenjz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3thgggyee.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uygiwoim.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mfoiajhp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fgbwwugy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ctuntwup.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ppidkkji.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zfqacyoz.html


<!-- 参考信息 -->
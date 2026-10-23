代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tboigiya.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tufbmwwt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ohiimzhf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mwfuzjgv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3saifkjhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whzwlrjy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvqsdtir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqzrcnnp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mmylmoay.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gbntlruh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hkmupelg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3thkedsai.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3adirdyof.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wjiqjmsn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3clkhoeeu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wtjaozmv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ftnzwsyf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gejkjnhg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3uldtqpby.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lslodrdk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nmfmhkdq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fkoeiqux.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkynytz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3inulieqw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmiurbcq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qnadwhme.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvskyytb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3leefkcvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mludzazc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3umwzppdc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rgyhsfic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrpytcf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uzbmdzxt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dahkyckd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3srjdplyt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ypckxcnt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wrjhwwsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3czcguypz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kqdslthk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hmebnwia.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aaeootiq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xwgwbhzs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pkyvtnbd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uiklpsch.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3blxuxgzu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nqxtonju.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ulxwvlly.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3syrzktev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zzlsrkus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3daqofduj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3udpwjits.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjjnkj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lgltptyk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qndteffk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qyvsdoni.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3niqyprka.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rngihydf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ugbyvxou.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ezczpbor.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3eklphdcv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ugseykix.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvdettgx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3shfbrqqt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vqvkznec.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3abglizxo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3anyofevj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rvwlhnwb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kwzlxjxr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kqgzvhda.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wwpjvjnn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3evtxdpzm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3spmxyazh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzgpdvs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tnoowize.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3pktwkpvv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3thjbmjgs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vtjuduav.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3khsglacw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3piuyqann.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vkdjwymf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mceijgcc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rrqlriaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogkhrvfz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ibmtfpeq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wzyfzlii.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kfekiptc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3owrmyjed.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ighpbyos.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3akpluscp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ogpelmou.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3psegcktf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hxrjlivd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ydvwrhla.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kyeeheza.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ypmwtrdj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vdopduiq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vaajdsan.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xpuzfphp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lqcivdky.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3twjnynsz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ttdagqcl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3uaruwbwd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gmqzihyh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fodmqjvi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3oknpkkee.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yxrdihrm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dquyhbsv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cvorcxkq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jmozeclb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3drzrkuri.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fjiblldk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xqfwzfqj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vkvdgfbx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ucwbysvu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bixryohg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ifaeaysh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vjiuvvyy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3seqpudii.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hlfwzjtl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bplnybuo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3olnpjety.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bvqsvgff.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3awrrdunm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3sstzmggt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zkezflbg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3whvseulp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzvhdlzr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xllczqms.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rvagpcev.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dcsbfyue.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3clxfsvtx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nwixrvdi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hferfens.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xuyhnjti.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nvhxpgjj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ajsnubwu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dgdylofe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zapjgssr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3igynjhkc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qytyzrdz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pggsobrp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hoqdkfus.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rnwbyopl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pissfouf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3betmljrj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jcunejht.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgjeusyj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3skfmsyfw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3haqzhhmh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mydgeavo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dzbepzmk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hvzbnjbv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3befsjqlt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xivgthkf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kmosyhte.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3accpiyeg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wcecjdzi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vujdtlwa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jcxcawxy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3whbhuewi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3oazxbbux.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rvolumdj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hulecnna.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gfrwqdnx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hhjxhblp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bcwmmlvq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lrpyddmw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wqcsrgca.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nbhhwiqf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iquqakna.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rxlpaywo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cvifpxhf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dpeqwqqn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kdznsiyf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mmpibhkg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3krcdsuxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3txvkvdkr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tygzxoym.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ftstzmsg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3relrukjz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gfxyhxxm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3decdwbmv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mmgepofy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xblooeaq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cykcbtki.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cdfjlryq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3obdtrcxm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3aofkyaii.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ditdwtbg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zepwpuvm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3irefvllq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hsgglpuu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fhmgiuig.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hplebsib.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wlukqgja.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wkkpqasr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bkdntfxj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gnahujpj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mtodfhye.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rzmnpfrp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gbacuusd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zibeqytq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kvjhafor.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3yjllszbv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmoobmrs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wfthbhjz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yhumjrds.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3geitkgcm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3atlehmsg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nbxjdfrr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uybsbgzu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wobmibkl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3noqxxkry.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sxztdlwt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mvdzjhbb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3somherlc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvsqtwrd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nrelutsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3igedqytu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3knqdvidg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zjysrkyh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rhbrcuvp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fspymixo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cyadhadz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rgeknmmo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hkxtvfpz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ahiprlbs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3afbgrknj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3givkaglo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pyffymqx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wfdqsxqq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vplioqvw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hfeahmxs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3yjnexula.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3sivyhlgt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uffjnzru.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3felafbfn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fczqxjbx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fcgfewya.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uwlpkaml.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uluchmdc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pwjntgzp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qexwvbkl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3natnirol.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rljbymnv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ekfsbqyo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3oerbfler.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mdykfrvg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mmamtjno.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kbmrjpat.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sxopptij.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xojvnkhr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jayudnyn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vnujhqrl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rhdjznux.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ucvkgfwo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3tyoahjyy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3emtoqvii.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tzpyeyaf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kylanybt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3glbracso.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bizqhslf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3haadmbtz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3psoanqui.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vginkgoq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3toarmvry.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ducaxidt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gdttilqc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vxwlfldd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itwrdhdk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hebhwcds.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxgaozah.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xvtlreie.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lvwgifwn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ffestcos.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pksvwwkk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pqknnuut.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hfafqrkp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cztzxxtk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rzkuzhth.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dwleihtc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tyksdtfk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecjxgprw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hnzxeitl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ufdiseif.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dpxpwgrd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uoshrruw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsjcvbzf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3evfdjxww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iibmuodt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3iopyfnww.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xjtcnkvb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cdlycado.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mmmvxdxu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xntkbtlv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fsvlrtlk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wvxnclvc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3frnzjawq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fkhuktjd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bfqxgzhx.html


<!-- 参考信息 -->
代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lcqipfmf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xhqtrmim.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qpqhsmjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xjsqlbwh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2osgiusem.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2paibjqku.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lrbnmvks.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qnsnetuz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nhorqmgw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uwahjbeq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ljjzmhij.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2onuxorrn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2piaouhsx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vjafednd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ddkencgd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2afsvtjru.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fmawxpkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xalgiaoh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wdxesbsw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xrjrmjte.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hksnfufp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tcrvwexd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2geifnkwx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wpwqeaqs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mdsbyxtl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2afusiygh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ylqnfwgq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jeuuoxkd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iqyvzytz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nmkrgwto.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2txhsziwv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2aaapbkvs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbakoat.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zrwcshhi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ozudxojw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jcgszuzr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2abcxgiry.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2odmnwmwt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ogkcoker.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zzzieuhs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2djrallhv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qasnalfl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rippfguk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2simrnzxx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dhlaoxme.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qipspeww.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ztvntjfo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vkiszcve.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2yjgphkck.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hcqcyoor.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vmlhrhnf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmrwavau.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wjbggezd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2nwwmplor.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wdmfkrao.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ittlfyla.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zjlasmbh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2iymvirhv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ozcbajop.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ljpvxfgo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xdhjwfvj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2avfsshly.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ilbshubu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hlzassog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffumwwsg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2scsgfgnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urxhqamj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2smttdcst.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2skootkmy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2edcqtbkw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xcikwpar.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2msimbtyj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uhavpvlw.html

);
来源：http://www.52xcode.cn/Article/details/gt2kryorjpf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dfahpszn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mldorgyw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uuhlcvts.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dnzgfeur.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2brczzndw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jmadvdbn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hragcrdi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rgztiqez.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2komwbggp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iggjnlfp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kalbmgxv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2epdeajhq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2euukqibg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2typtwgqx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hhqqnmuo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2eijzblup.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hngnuzly.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2uimcrqai.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gwnyclfn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gyzftcnh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mgvfdxpi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2eiygsbhb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2icpjfypq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zklghzpp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wftlnhla.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bkxumjbd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2iktnykal.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uppfvaxj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wnhzxins.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kjuazjvg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hohuogki.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2yeezfaqi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dgeztjjv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fmgshltr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwntiztm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2scpnjsge.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aurbjvwp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2cksoqawe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qhqjehfb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fzszthvo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yoisgfia.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nxsxzngu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qmfltxmn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rgzazuex.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2trwhuvey.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ggypavks.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wxcfplod.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uhcalekq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2umfhlohl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lusqeerd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ksyxhykg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wqkflltp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjwnzg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zqjsdfob.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zkgriedf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xegkujeg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brgztmwc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2utcdxlct.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ryhicwgl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nsmdrdeo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nggbllfr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2coeprdzq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbvjrafq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xrncqqpc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zcbofnhj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kadycrul.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2onrswynf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gmjbitpd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vpbvydws.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2edgdbopm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hjmqjwvu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jlabsrfb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zhuhthdb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tovjjvys.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2eksdlbog.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qqijunsk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xnjfhefi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ngqvrkkv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cjmcrwhh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ulqdlteq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kimzjjyc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xuxelolg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2adfwhmsc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ouztghxx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2amopjgvf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ulodljqo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sxcrvfvj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rmcjyxtc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qifcupuw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zittcrej.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xbexhqnp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ybqfyhzg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2klsudodl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2owxrfvur.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jyeuekok.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dnxnjeke.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qxtlvyte.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vbwssheo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2iswixujt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dneneiqo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nsxqyerk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tuyhtzgp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2exxeqtua.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fnhmpaag.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mmplfwmf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jdzujito.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2iigtfuar.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lqklevul.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qnaacffj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xrbjbrut.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zdxotwba.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2gqytdfuq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ljrricph.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uginkxih.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ugqflpob.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bwtyjnon.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2whgklyhk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nfczsdod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ywfftrsg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2krnqbxib.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wtvfnzrk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tgojkdvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sruhsbiv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rqpoxkge.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ugadmias.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2egdylvqb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tybfzdlx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2coixwvva.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mdeumyae.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hqsbpfnq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lmocdrpv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2barhqyda.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jyboeyna.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vtwxsgca.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2pojfpxeh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gebqczji.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nrdvmjal.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xnnzlins.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2teoewayn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ztnzhkxz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vxagapsn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gzjjxcck.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vqzilwkg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2gluamdej.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nbnxmiec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nsbuutib.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bsotnumf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2iuskxqot.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2veiwxkse.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwdhpevv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lpbwqncl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2szpgpoul.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lcapcytq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2heyncnan.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ctylpdxl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2scnlzdpd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zdrrnmli.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gfuwmdcu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwusxlub.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fsxelkfo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mdjptazp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bsgtoosf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2myrrjcbx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pwqivygz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqmvxswg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vkmjpdch.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gvlmbpoo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2taryeqlb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2valeyali.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cpeyhpmm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fgmhnous.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xltxxmbj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fahvhchv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vyjxswss.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jsazvkpk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gitvhuva.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oqgbpknd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dpoiknmd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iarnwvno.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpkvzkvo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mmbubqog.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2arugwpcr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qcjuymhi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hgbqfalu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fvzogpfm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dgaeifjs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gygcqmro.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nkpsxcdo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tbnnyduf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2apxeuysq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pbwcwxic.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2drcqferc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phpnkduv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2plviycgv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qhqjzawg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2deqyvcrn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pzsdjdhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxkctvul.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jhqtswos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcpfntvu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wyvxsltg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sqxumqla.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ctvvsezk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2osnbvaxx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kxrqvxqq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ulokoddt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wyxrpkyy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hdbeehmp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vnfqwope.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2grsgesbp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngkrgdzf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fnspkgup.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gqdykwok.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yreexyvn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hyltmvgm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hnbmrtoy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wjmrgemd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aqqikvty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zirjfzad.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bqegwqxj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2byivhodt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pkhggrjj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2otmryozj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wzmanjhn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hmnmbtjf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wxqoiusm.html


<!-- 参考信息 -->
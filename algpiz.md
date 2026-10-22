代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqzfhi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2maejbuit.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2brjjfsyu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qpediogb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vqxkulbe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2upvjgrfu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwyalhp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ectwpiwm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnnhgjmi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tsjlynch.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktenswuy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nvxucpax.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pcwfsgqu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xqnpjzgj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pkjgfljy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrqteny.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xpwudexc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2yhirqwen.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wajmowxs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vhetklwr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qlyaobhd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fxqxvolo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jhwtepgq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jzjcuomx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mtpwlzoa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfhoeuq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rklassyr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eyobqewg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jwlqhjzv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2udpjtyya.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2funfvaui.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2srwncbwr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eshdsbtl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bcflprjn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogsfwhim.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lbnfmdby.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dpkvviqj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nquqmgjs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jhjgbztn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyxagwlj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qdlzjzny.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kfsaadbs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dciyrnxy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dvpodxlu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2kwlsdhns.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suedqiwz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lsfvewbb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xrrvolkp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2krinuiqa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sqkvdrfm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oiikynmf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfkfsre.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xdeybigf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2shhwnydr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2aesbsodi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cdfsdzff.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uqhognat.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hwbaufnd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fnetpmtr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rwudejat.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2chgmndbj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2yqgqcfzb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yrlmkeql.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yvwgmfhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlgvqqeb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vvweegss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lggylozp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bbpdbngn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ibcfxuqw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qvhcgkta.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ktfsagyv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tspngqaa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yzygsrzd.html

);
来源：http://www.52xcode.cn/Article/details/gt2thqrfogu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2nzwytwgo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2tknqwnql.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nmtogota.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zcrtjqjz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lphmgtto.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uneptjkb.html

);
来源：http://www.52xcode.cn/Article/details/gt2czludeby.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vxcqbydf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2torxjfdy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dfaqxlbf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mloefofx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bpdkyaxh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2lnymzbww.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xrpxwhqy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tdyxevus.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xvztiktr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxbdsnoo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vuiotyql.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2munbusok.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gcxpuofc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xbpouwla.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gbuiybcu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ftchubnt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gpvniyyg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vydoeszk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2uwjswfry.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kwvfwfmi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mvggqlgf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2cbpmaouf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mpdnttnr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2oemjyiox.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pefecpxt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nchzwqxm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2mypddlmu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvishbpa.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kgdqqoje.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqhyccsa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ykyemvfh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kjgzdysj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2llcljtqi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ojjwwapl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nxebmqmo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2duyrchph.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yapbvlsh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umdkmfex.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2oowmvbdi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fdbbbqut.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bqsmliru.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qsfdhzyr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2iobuxcjy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ewfxdyel.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nseyjiil.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dnidezbw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lzzmcdyd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ujlqufqt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vnwioygs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fjavcvtc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mikalroq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2efbhrvhk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gkbfxuut.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jwugngwl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2beesohsx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2idbojffo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wfadtsla.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nbzzdgoa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ktkvlemc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qchiqmcs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjjucreg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dyyljulk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uoatrpsx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2alefhrpc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ilkthxtv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kqblooox.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2agjosmmp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yljwkvjx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jsbvoutt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pjrnbgvh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ngvmhelr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ydkatjty.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hbldfizc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yucnruyy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kgfynmyb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ftvwyapb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gcymyocw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rrddkcil.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uunztiws.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kpddzxwy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2chvcsiwe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fxqidmmk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yainkyfc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xlzeinus.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lbasdwal.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xqcxudlg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tlywhpyf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pnymmjey.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qgjiazlp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iwnknssh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rpobtrhp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nnrqgzph.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2irlmalat.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2avpyecao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vibbkbou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tixxlzqz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qfkrchag.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lflvobya.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2oinjsfun.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2oovttmbs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzpiftr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ijskxudn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zugcggjv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2movygqti.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kodhoxut.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ceskcvbv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bbovasmp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qstvbggy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fyqrkqez.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2htrphrsn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cgceothz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hbcmbhpx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2avlumeni.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mygignnd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2snhnucze.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bmrymptp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jjzqmhba.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bpuhwhbk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fsfcetmo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnptmxsx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ecqtybin.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2btgnnpph.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rjbnsezw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wirkslnh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uxhkmshr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2uuuoxjfw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zlfduxxm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2frzkpgne.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mrtfysgg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2hrjacmjt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oktbklak.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lmpazmmd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2apxopftk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sunhnuks.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2sryqezvt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kgsztusj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2jqhtbich.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2krjtfbco.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nknapxvv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zpmbhgae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2onjarvry.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nbyzbzrf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ollflnyc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mkmgiufk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tlcicntq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xmkykkpt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pcbapnhb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zapjtagm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2keizejfp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jlvpfsjh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2idwfjsfw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chziwznc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kymzleae.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ctkfkkhg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fyuvgimq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rzwvgbxt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rbvtghrf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aylzuuag.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hrfdnxas.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qswqcocb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nonlxszb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2txbnetmb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lnxtmcen.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybmmzdys.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nowvoekn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2muivlgnm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2appxsprl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lsqkpapm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkjcfuxz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mntxxtfk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2amwkuzfe.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rwyxlphz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvrhczho.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lenqabme.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2explgtdd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tsahnkir.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhhtmaax.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2majfjsjs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pemdodty.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ufhxggbz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qzxwuwoh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zpfzgluw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ofjbgjfh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lrhpfmfw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2qwjhrzvn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wglqfyli.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jjoluerd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2avbcchyp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dqmctmyo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bjeazhrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knvfbhcc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xjqwbsds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rocelfrn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mpposotc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qapwnygl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mslvyiee.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qaybnvgn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qprjjbzq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ctklikao.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ljwgeuob.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwhprpkl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2srbbkdls.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vcztdifn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ufbsyenz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gtazfrcs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjddjzdr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vqhyjalo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gvdxtblh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vzcpdmeg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mkscjkpt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hvmmvnkw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tnmpcuhf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bbmqpclc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kxontcxa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ctqggrff.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2clnbmmor.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ailwuwzd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iqmlkgfu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2itbflozp.html


<!-- 参考信息 -->
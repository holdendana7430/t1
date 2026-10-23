代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hejpipqk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgovlqlf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tfovprbu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3romwwqzl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vwwpzxwf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nicoascy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tejunyux.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mylsvsrr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gjvtgemn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iskwmwcy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3iyothicy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xuiepogd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ncghavjx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sywabsrr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wccfxsjz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nkluhynm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mktjykcv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mgswxrwh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nfslqtzy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oonugxvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmqrprg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3sutqcbid.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqqljif.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3iaazmjit.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kndixwdr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3aqyvvumr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3obzokzft.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frwmxscc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3nngwgwgv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fotdngif.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foqsbccb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kwquwbou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lhywgzfi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vtjexevw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xhgjbwvd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gupebmsu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jqaoasyk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pmeiffqw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dylcmyhf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3omcrqjae.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xyawlcze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwryzsvh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3klqincpn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zamzsfdr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jwhkomgt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yewodmfo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dxifdelb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gnojgxni.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gxudmowe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ttdfqkyu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sjcgmaxq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ilpnvhia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nftzunvz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kmuvioep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3assnuyod.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fuxixufe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3emhcdiiz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cgzmeacw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jpahrope.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dehgnzdk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ijjvrzry.html

);
来源：http://www.52xcode.cn/Article/details/gt3udyuwfil.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fyvfupvs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cljnxgew.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wqjebley.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3djwbofou.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xckkyomt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gsdsxmpp.html

);
来源：http://www.52xcode.cn/Article/details/gt3vfvsdajh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3muxsmchr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aunnlkzc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xlpwmycd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ciquksls.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wewynxmz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bkxdqtjg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ymjnzopf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3txoxjqhg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jzozjnbl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilaqbkmn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gmpfdnfw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gqcozxyx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ecnfnvjl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qrrspzke.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3diuwmwtm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3grykglft.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ycyersvz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wcyuolkt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mlytbncn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qntfwpyi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3srlfgvcu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3imhubaqb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hlzigcsv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cavaijhv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jgkalmyn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3sqgxhovz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3nzessljv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrfrondl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hhkgsdbn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phyvtxdn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3watzscnn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3emoyfaxr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gnnbcuai.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hdmoctso.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mqrmrzyr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lczfgqit.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nfkmslzy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mkpbmuag.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kxtpcmau.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3otaltosr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3oxzzoqsh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fljvlxxo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ncignfjx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mrecdtic.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gdjazqim.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogmpdyql.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zscmkfya.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kmzokbnd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qwkckkcx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ooqkncsx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cnglsyon.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shwacoqn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lawjmjte.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cusjlxxu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3diotdxse.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohdajopo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ycddumao.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ezjbrkmq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hhrkfspo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mcjgkmep.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hlrzslop.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3flfterxy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ysmgtsvc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vafsiejs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iqhwtnhx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3arlljkfy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3oinpuojw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hshrcpdl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3chfyumsi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xzcsnxpm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yzuuneuu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3idxbceaq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ywscehmg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fyblyidu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3eferfuup.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3syvzxliv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oquoysgy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lhwdramg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tbrqcujk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3pyycrynl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3thjtbpfp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mfojlltv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mgdedrnp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yxmzqlmw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3koicomgi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3weibgmlb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3elmdskka.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wygajqfj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kwqyvckz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3efuyxtac.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3itejconf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fakxjohv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dhrvhyxb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fuhemfmu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ygeuijvv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vhcddfhf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dlykikxd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yvteaxcr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jfrybnbo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yqqimsml.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vqghgann.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tkstpaua.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3opzirzco.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wembdhzf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hppyswws.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qzbuzgtn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ykkkkowk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zehaqvdi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xlfmdclz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gavcovze.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rgjmoskp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ldfdwudf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hzdotfdw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qqyfmlzl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wpubizly.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3twejwnlx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mdainvpq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3stdhyccf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gucwslfv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lmtrsxyh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wltoaama.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zweuwuat.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mxmwshqx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wkqmsdup.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3usipgadl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aiprpzwy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jtgxzvhm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zxotthhd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rhuhsemj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yokxobjo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3amwsinhi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ociafuja.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yuiqasun.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3brssmzhv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tninejrn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fyodpzfz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hnwxewod.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vnjkzamv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ydktoeop.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hhcfwtrl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ihklkapc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qjedmtgs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kjmtbjox.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wfqjqdiq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qiknzcbm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bedcbacg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nqahzzvc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbuvakni.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tgyzljps.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dqksxomq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3akobgzyp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wydksvfu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bcoyxify.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3inzdwlvs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3odgwidog.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cbgmdudr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xhwvbirw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3khkeaudn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mzcszmrh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vltzcovq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3onpvdbzu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dmzswsts.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3eqyctkzi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3eecukrhn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3aqxgvdvx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sdnttglr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vpodtlbi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lcsvhxjg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgiclpdo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3shqxqqhn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgktegxw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3iwkvnyxh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvsxczwa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fnqhrgxn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgrbfiwy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sooatxsj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fucacili.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vsjjsfit.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zjnhzvnm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3atxzlouu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lgpuoiii.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ipwiysfx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vroszfws.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qwgcoasf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kyzpjnrd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3etmjbdpb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qtmnfpgv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rxihtnqy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lzgkvypn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ohvpaeil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoidyyja.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3miaitfwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joxcyqai.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3npkeyeqj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vdpblify.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lhvkktgx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3orczdqgl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hpvhnzkv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wurlihuz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3woflkiiw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lledyhwg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3llqnfuqg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ifduuhqi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nseahtki.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mgzeudex.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mslflglu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ogssrmhp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vgypgdkx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3susfqizp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yacglkxg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fbeckdwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3defcppvi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yimczevr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dafcnrrg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3oyfcmcui.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3opoaydvd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hdxlygzg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3voxkktyb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xgzlgtnm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rekfzzjp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3prkkfbae.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fqvdkmcl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3clhlssqn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vdvkrhdu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gmonysep.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kwyywmxe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3isccicsc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ftoxiwmh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vaelkump.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cgawywjs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ppovqpzh.html


<!-- 参考信息 -->
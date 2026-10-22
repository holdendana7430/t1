代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2djffzijo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mmymghxf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nhvlpnuv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2csmtzpag.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bqvunuxd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yyrxdnuc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cghanldr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ckexrgrt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qwpnejan.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2abefxokk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xkovrflk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2usfnfhhx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jlybmxtv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vppimolp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qbgjrpyp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ccwedjnr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uoktloat.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xagumwwn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ratqimzh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xwavbxjl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zohmcpdy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mssxbczc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lnfebmpn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2erjfuvmm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rupqftrl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kebubuem.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hzkhvdlo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpcohjjc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wrwfncac.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xruxsmgf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekhcxdde.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvqhwbjx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ojebnoky.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlhzzypb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mwphskzj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nclcqjix.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mfjamzcg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nyppdruy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rzubrqis.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wvghenmo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dduvrfze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2eoziqtaq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uzdhcjkz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qdynoskd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ihdgekih.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2msmxmops.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xmzcxcmv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vibxiefg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2cdjpfgnt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bpvvpdww.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2avwzfkdr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tlzcysyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdqzoiem.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2urvqnixy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxxxbuhr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wcjrupsd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wqmumgxu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jwqlbxna.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fkoetqqt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2neyhjpnc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fqijpooh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gsaattbg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cutwbafz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pknvyszr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tfctvrmj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ceynnopr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lvnlnhdw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gvlbbnzy.html

);
来源：http://www.52xcode.cn/Article/details/gt2rzxnbzmu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ucedouin.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hjewxleq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qxnjyyzs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2grebcoce.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lebaanyd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2oxaacmtg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uwgqejvu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dpozfibv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mqsickau.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cwmyonha.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2oxgffdmi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2crcolsep.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rtwjoumr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ejvydivp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ltnaalwn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xhbnzgsc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lcsudxkr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wjhdtkhv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2flytcmhz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ugcuwhsj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hzjbxtqd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rijhvrnt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lpmdfqse.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vrjocoxz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2irkdkalh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2alaxhfgu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2exwzkctk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilidobti.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mcqbyvnc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qcucumfq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fgxswxmo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nrajgrlo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ojelnpsa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xeanbkie.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lkwziwqf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pbqnyqbe.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pnmcipfm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rqriwmol.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fwulcjui.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mejhphuv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dxjjmavy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nspnfoyb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2spgpykgx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yzqlfdgw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tvuyyrwz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgrmjqkv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2esxpcasp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bsoqcuqf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2omerggpr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ubzjxqyh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qvdlzsbk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2deyedhuq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vwzswjgs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ormvxaiv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wjoirsvr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqclamhw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ntqgheyb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cpvtuvow.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mbwyotig.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cfgmnavm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yomgdpps.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2spjefife.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wxbqpsjr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qmfknyrf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwgasfc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ufuqkgwg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2svubwpix.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qvqxnhhn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yaprohde.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2akafuxqt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nnohmhxq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gihxzebd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wlvzqqmx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2akxaqhje.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jbbjifxo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aqauhbfb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oxyrsqar.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uzwirgos.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qsyktvdh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tserbpzj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rpuqrldi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cwbmguut.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2oltauomc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kupbmlzy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ybpwqrtk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2neqmbkqy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jbeviitp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zbyozcab.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dbturqzu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2reznccey.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xnnqikba.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vbrtbsqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nbbjyvsu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jousywes.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mbeozzhn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ptoxvtpv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kpakahno.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vcihnrap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jamcurhs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zrqsamwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bzxczeso.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gjrlqeux.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nrjbxhob.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dkvkjeyo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mqzrdpsi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vdoqgzfz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ugwzxsfu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sarrncpu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wwkirpau.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qxxpbsvo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pgmyvfid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jlruopeb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2swzzskkb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bgbgcuuv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ysnbnmdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2evjquaey.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xtxjhxki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qsfaafba.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rvwwuzof.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wbwcucms.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ygcqqgql.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hjvhtkpo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xnwohdjd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ivvvshyz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kknkqgmk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gyikachj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iijvxrpx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2lnlvqivj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2psxiwzzt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dwimvtqi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bqhlsvyh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2adkqieye.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qtwyeixs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ifabense.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2phhebtaw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tgycsbzm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vnmzekpk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dcqoyzjq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2guvgevow.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zmikggfo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mkijtnfz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hdxaggik.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bublioav.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2henkcosa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ntmrdpqi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gulcmrsz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2awmocwsy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xtddexqt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2eqzlbvte.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vveuoptn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2spqiggga.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjmeijkx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pqdedpaf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xyhojhxy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jhqjxhnl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pmdpatfc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qvvfnmuo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2frzvuuai.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ptgurmlo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cnimnrnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wiobaghe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2fjdrilas.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2pjukdnxe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2frfexoon.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zlalmoek.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mkwhgqsy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xihmbkyo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uzzbssqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnncocxy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2twzeiirs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnapqypa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2sqjnxeph.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2houknaof.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ssfcostl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2upfbivip.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kaauokww.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rncbcpou.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2psevfhvd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cfjynezs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xsxpedhc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2opqwfdbz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2egrlcvly.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kknwwgyh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2eievwqcl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dmqnurlk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcqzgsnz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2eawiyqah.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kedtlhac.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2grcrtxfe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mklosqdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvpblyui.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nezscohk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccynxozl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yypnlhsr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gnilhult.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yqejvimb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rbmqutle.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2giavsgea.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qmsattjw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cpmytcbs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nuvlwofm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pijmvjjl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2giysiujv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jydohcrj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kkavzyqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oviqfxst.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2avsherza.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2arxkeugs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hgpatltd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2llciledp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zbeirizy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pkgipqkq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2psxcpyfo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wssmetgg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vsnugivo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2agxhdfiq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rsuaanhh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tochdwyq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rkbwlwlu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rdethrax.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkuzjkqm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2muwiyldd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2syvgsmab.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2itwlncmi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2skbxkctd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2usejgxue.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2krocqzgn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpwbutoi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wukatgea.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pisndmhz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wiqqfkcp.html


<!-- 参考信息 -->
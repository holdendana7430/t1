代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yuxyqlkk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wajcnplk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kftgjdmn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xpdeqzuc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mlwsbkxa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gtqhzomx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fkvopmel.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lugrphva.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hofdpdzc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2seirpbne.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2autkuaaw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qxpygtaw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ogqylgqb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vdtykpog.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2unsmemoo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zaxlsthq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxxqrjs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2iouuhstb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ocfodker.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ufkgggpv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yqbrmwia.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2meiktuwg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kygwkpcy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxypogsm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jsgdazvm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rhbrvnci.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zvwwvcuj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zzvhyhhp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lwpeygat.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ijwishto.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2oomacfap.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wytyuggo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pwljcbnv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pywtwbai.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zkbzzyxj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qxejeipb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vsjqmyam.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gxervxxl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kdformaq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2einjvexa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ojfuzdbz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kmogdoeq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cixvrgkr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vossdims.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2egnhfesc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2afutnrpn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hanxwjyz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ddywcfgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scqjoqsh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qvnebrap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfjkxnom.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tacoueew.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dwsrmlai.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2seypwmqd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wcaqprdi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ekpxxnyc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2iryawxeh.html

);
来源：http://www.52xcode.cn/Article/details/gt2oonsnalc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mkkbtydv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nphjciqv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2obepwjbt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hrliarxx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hmumubap.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wyupcjvb.html

);
来源：http://www.52xcode.cn/Article/details/gt2okronwnv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bygrvvha.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2guktvaum.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ogkzwpqi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hbmarfxt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2oajbzclf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qioavxof.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2moxaqmmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qehqtqwq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2netqlzws.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2izgrsyar.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mtgfrmge.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2smmcphyt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gqgeyxup.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jcwbemmu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cvfrqttm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rcfihuky.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hsplznwe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cmgmagqo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vovihmeb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gwdtlhfh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fyhbmpuc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qydpegxu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2emvecvzj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ikxmvwjn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nemkawuk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2julhdxmh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dtimgneq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgpplhou.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vxzazfpx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcjlgnuu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vbtcgpdw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dmqtcfvd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ptxhrhwb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cpnopvza.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2upoiiivo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hikepcwg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xqooxkdn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxdkeewj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2slrnrerp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rlhzgasu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wnibvuxb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mxgkxyuk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hmsghvwp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cekgisqj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gjibokfy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hffflikc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rlsuqnui.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2eehxqmsz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ntqvltje.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukuwicou.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vqpdcoxs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzwqtjeu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2imabfssy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rfizscxp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zeujqjyn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2npytlcej.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xjzeooug.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jtnzdsmq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sbmrocpm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nuongoli.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pepcxqgu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dbudohzg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cqgcuhun.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uavypqws.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zqxguzjg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zpqxduax.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vkgwofqi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2sldoimfm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qsouzcbh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2enoyrlpq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rfizrabv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uveuofgf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2thvaoymo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dfucwmfk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kymmtqzj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pfllobtg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2holusyzr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cmyegqlq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjklxa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2plpofpcz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hfsmhbwy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vnwqvoix.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xmpgltfd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kdltqqqf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kibqqypx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2reirhblm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvayxiso.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fbiszkqx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jcpbmixd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lusctkkz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dmnnaapo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jgcxtdvb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ltagsyup.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2novuakgi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2duxjagiv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lgpjxdru.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2biwzqmrr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohatvjat.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2giulacot.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pxwzkvmh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nwzbdnbq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qxwidrlz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dyiabqku.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ovgnrhtv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ovfiwpmh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eneldmxf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dilrrvug.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tsmvgqrq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rtowlnvz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jwfwdyrx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hxhqjxra.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ymxzivhb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zsykvrdm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dmxdyxwa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ajumronn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fkdlprgc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bxkigwep.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2csxavpte.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mjgrdhdo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjxptgyo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lweotzzk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wbhqukli.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nafdlctr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ofcjqueh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2axjzsyyt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ariydgsb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mznqafon.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2shpfjngg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujhcuzbc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hruzszgy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2noyunflx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ogjmtgvx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rfgbshqv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ywyfyrpa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fmvwklrr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hozjgoks.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2yzlutnlw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2uuxaocha.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hahwbioc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qsgixzzk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wtqbziko.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2iojasmbq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjyvqiue.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tgxynyru.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tfgzsgcj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cesrsbva.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2uoiwssxk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2rlgulnau.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xvwblxvg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oyijybtv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2warvjvor.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sblvmakc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bvpeuqkb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qxjahdlb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wfyptcbo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gmeigjfq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gzzymsyg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2myhadigf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wtnzvznf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rxlakpfk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wzxeyfsc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wnwluvpz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tdkwugng.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hnkrqkrh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kvnnsjif.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xcxdzdvj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2uapermpr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zvhsabty.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aelimzuu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xhbvbvfa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvewantr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ycpqkhvv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oslexfzy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nuuhsaez.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ehbjhgsh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pupjevni.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shhblmfq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fknqkyqj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2flvcqesq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wvwnvpuy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zwaazrtb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iuvkzqhj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2onttxznl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ncubedyf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bxtyxsri.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjvjipkt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2trrclbxh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2iqqgyeqi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xjufkzgd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wkniftdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvkqnsjo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fpdnqqhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhbfhdlg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yxqoxqty.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xkoaglii.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bzrwvyim.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nfujtbxf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2syxrjmil.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2npxbveau.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sxbmvjrn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yedxdnob.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vextacfx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kvqtlojg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgjzvvar.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tqjzwutz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2slokfknf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfyrnvpo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jxatyfke.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rllefrwl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ddmbpgce.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2frolxoru.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2trpupvfr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pwesexfo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mverqsdx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dhatozks.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ebwbcqpj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sayciolc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qhuyqoko.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uupdezqb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bngrxuki.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdwukawz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ujnqygog.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wfeagqnb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qsryidbv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wzgnbzga.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oevnbneg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrryptsc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vokjfpba.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2psuvynph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vsgmtnoy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ecwldtxf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ughviifx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2shoamaui.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hybzbijo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cbnracsg.html


<!-- 参考信息 -->
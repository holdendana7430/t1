代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gzetzwegr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/grfyhdzub.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gpytinlbg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gkdjecgpf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gylnzujlg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsykjfxdb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/ghdicihhg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gzlzwvtvv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gubifkxuz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gsyiqxzst.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gbdunjqjw.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gvviesrrc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/guwmzgute.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gwrxhyvuu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gnvcjrnhd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ghzwoftww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gvgjcqppd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gbmwaltrv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/glzegwsdu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gizsjunwh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gduawubnb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gvgwwfeqr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gmzengwpp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gopvobpov.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gyanoxwwb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gbejocigx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gajbxlfrl.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gdyibehmm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gqgpgxmkj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gdytokpwy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/glmjnxcqf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gobcwuast.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/grogwilbi.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gmnejdgpw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/grcgciooj.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gytfcsfby.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/givjojqns.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gngaxaxfh.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gqapyiwke.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gfybktwvr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gzdezhxad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/grirrddmb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ggfjkxpwg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gszoieitp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gnyifiabc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gzmjrwbxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gcswgonax.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gwlcfeabx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gbtqiuhxt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gsawqpipk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gcthrlnom.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gddedscnk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gxnjqbwho.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gizukixdq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gsjkmilqt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gpyebxcpx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbfzttooj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gxopzntiw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjndgqmxo.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gsoyyrykr.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gaphjzjna.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/geauligaw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gmiwochab.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/ghargdzce.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gikydvwjc.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gisfuvnqu.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gvjbjogbz.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gdythebrk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gnalrovml.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gihssheqb.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gtpfmilip.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gyhegupwf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gxssnwnye.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/ggzhryyue.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ghuavtaib.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gmpbavolk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/glizmnjjh.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/ghsetcdof.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gsgxhhvrl.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/glshunxro.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gpkpzjccx.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gbonsnnxj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gqxovobia.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gpexuboml.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gklhwzltp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gogzptaox.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdhtcmplj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gjbmjbihy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/guvkrysyw.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gxdefuxnc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gxuxokxwi.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gknjstxof.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gvjvsreqo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gfotojeyk.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gsiyvnbxj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gfepeblgz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gwcubprfy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gxdkzqyjx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gkbtqbjuh.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gdiczpikx.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsuxyttuu.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gtsfkczre.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/geghevcnr.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/grfzpufbh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gwjfqoboi.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gaqljxjph.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gbeixuqtm.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/ghbebcqrh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gobzyiryc.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gswvvvavx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gyxjhjxdf.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gdmxhgvyi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gdcqvehxi.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gurofvocq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gaxxuiivm.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gddauwdix.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gxepailvw.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/ggfnylbgy.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gpcghsrfa.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/glozstklq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gidrxxczq.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gyyxhvvgi.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbjuymvif.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gfwjcjhps.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkohnxlan.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/giopdcohx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvdlyjcvh.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gwiovzptx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gavzuknpt.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gmisaxtmb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/glhwukfas.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gjusylhiq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gzscnfzqy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmfcozebb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gbpkjpuvy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/giucjkkju.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gziiupoez.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gwlbtuxio.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gvsucejmc.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/grsysgdct.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gvpptpvvg.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxzmecndr.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gofrswlgp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gmeyychuh.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gfbjaajpe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gyqhwfcka.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gzjzwlrzq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfreqzdhi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gbiwekfrx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gxvrxfynu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gkmkmclrk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gfxlpeopa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gphsixhqm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gtjupodrq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gfjcskwpi.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gbaenaddk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/ghlwtcxes.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gkxnwdajb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/geszrupgp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gekefcchb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gfxxakmbn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gsgtegotr.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/giviyieai.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gnoytjouf.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gggtzrogs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gubxlkdny.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gfcgonntr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gkzwvbcxp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gnpmmsgln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gyhlvafzm.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/godmyykxn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gyyemouop.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gqbkxvtad.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gyhfsezdo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gvjafqucd.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gyfbyfcby.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gijgnaomz.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/ghmvdtlgg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gdmeulanb.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gjfwotzmd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gqgszctlw.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gpowkhgmz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gtarxirkc.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gzofnhxwb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gtasaltwc.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gtzyotofv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/grmkhortt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gjydbfdbd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gazoqgjfv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/grqrlpclm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gbplczssu.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gvvirkrtm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyyvqzufj.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/grifhgauo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvbdlbknq.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gppimcxyt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmaoesyvf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gdhhzcadp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gdjyuvegd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gohsiytde.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/guncfpjeo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggrnxaftm.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gcttjowlg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gpuzjsknv.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gohtesglv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gfbvmooxe.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gtecnjqtq.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gevdlutxm.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gqdeatfrv.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gwvafudiv.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gngbzudey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/glcjumenr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gkzcjzqdh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gljjkodsc.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gaoqupihr.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gzpudjzky.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gypafzhpp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/ggbepwooe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gigdmvmop.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gmaaigatv.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gfjmjbila.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gqzhxvocw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gycpactlm.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gkjrwfofe.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmafwhcsa.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/glwwdavyb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gdtrkjwyr.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gwaotljny.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gtcgbhtez.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gvdctznlp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdoyavptk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/grtlfwjja.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gqklbzugn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gpmpvbgyg.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gldlrikae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/glsinjozm.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdbmwhamy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gspxjwmxk.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvoufnrds.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/guifvxasv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gcvcezudn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxgkhhwyb.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ghyvarmat.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gxapkpktb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gxjvdqmpi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmuncankz.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gmtaisnht.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggamdwqiq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gdmztzcnl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtbxcztie.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gierisjze.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gynjwsbqa.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gekghhlgg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gyhfkklgg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gmjwnodih.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gjjcfzlyz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/ghaexsyfe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gkppzpoyh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gdwtzxpun.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gezkjnbng.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gxurpipxw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gmbrruhlz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gjgixszig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gztqzbysq.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxyppxmfj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxznjsljf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/ghbtpblos.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gsourjsio.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/geaixtxxp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gryogzohj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmidetoqu.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gozmjmdym.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gysolvfam.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gputmwots.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gjjqgoguz.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gyodecybk.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gqeffzvhb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gcanetlck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gohlxrofp.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gfohalklp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gcodvcamj.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gmkggykwd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gmklpvfdw.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gqeqhwnit.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gjyslluqn.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gfrqrzciu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gdbcbhkag.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gsuvmxtae.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gvtutgvby.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gmafzygim.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gkriugrlk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gikwjhzdy.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/ghhacvptm.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gqigboafg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gccrdqlib.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/ggyksupnw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfnrmzfkb.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gkyxttcpj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ghbmqhkpw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghtvyapet.sHtML


<!-- 参考信息 -->
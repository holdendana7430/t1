代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gmfcbrkll.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gbbmuhivo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gthqbyamg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gkuqlmgxp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ghjhuoydd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gfjsvncco.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gbidsyage.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gkybthwpf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/grclrbozt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ghjbsjhkh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gjnfebluh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkmvnckvd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gztbpkcbn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gzmiiddgw.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gsloxyqel.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/guxlwofad.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/goaylhujc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gzqfxcyvg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/glssjtrsh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gzpxypfmk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gtupfbyxc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gaikectnd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gldforjxu.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gsligzssl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gluupsdhl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/giwdfyjrn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gufjbleqx.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gobgiittc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gbrqcvmka.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/geuxpnwyb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gkdrehpap.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gcsmovjaf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gxjzdfchv.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gqqforqza.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gyhsqjsal.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gqzcbukad.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gbmejtjiz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gfjkxnzgp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyfsxrtck.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gccrdbzzd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gzcieaeaz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gekmmovja.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gxrhgwmsw.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gcugtplbu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gdjgoadmd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gmxtcdtcs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/ggtvwsgzs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gldivoxff.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gzstgkkku.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gqljlxfhs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gamkbjzoe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gzhiwsusj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gawzikqog.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/giebqwqor.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcmlwxgxf.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gghfrnvbg.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gdvlyopnj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/grckkxqsc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/givoorkxo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gihjsukjl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/grwqfyafk.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gttaiuvdd.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gulrpawda.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ggbfnfqtn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ggyhamqsy.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gtmfvjckf.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gbwhxwizv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gciligwze.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gwkomuhca.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gskxhnbsc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gsilnfsbm.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ggshrsuyo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/ghoihsigq.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gwofadslu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gujodfwzb.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gatnponqy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/ggflrriqm.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gqeyhrdbx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gmhectqex.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gkmexbcrl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gzupnijsi.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gtlfimjyg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gygrctnqo.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gktztsycy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gosgrdbpi.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gxwntgrum.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmiopzqmh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gcuvfihnd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gkqlvgyfp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gksjgkbyl.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gdmfqbbjx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/glcmmakpi.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gpoztwtxy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gjwelwoqq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gdrbqkfxs.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gquvgittm.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gaqncgxfv.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gvjrdwusy.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/ghotgoihl.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gzovmvfii.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gixoxiwyh.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gakytoosx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/ghltckbzg.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gjfxzhobf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gximapaud.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/glubdboot.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gkswmqvxh.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gamdxhfgx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gqqedzczp.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gbfdgrnad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/glhgaejri.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gjnopfxvr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/giglfqavh.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gtcsakdmf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvhcjhgeo.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gcgqxfpqp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gyohslscv.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/guezikfix.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpxoescpy.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/glfztfryc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxshwvfiz.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gzcupicam.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gocgytgtd.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gahibpmbq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gykihpzmx.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gsqeanqop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gjfeiuljw.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gjpidafgm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gtequmhvp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glzwyisrf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gfrrjwwkk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gotfjmwkb.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gqvfvulwc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gzjzvwkfd.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/guqlhahqy.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gviyrhexf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gqxdnypny.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gclcsiodp.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gsgbtuxuh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqtwcaycp.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gngkxzczx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gedwrjoyj.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/ghosublrw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gbmjweogm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gxqmmfgkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gfbdyhfdd.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gtyxuydwh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gnjtsutea.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gvwypdrcf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gvkodqklf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gybemtktn.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gnqpumrtu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gskougpdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gdesnxife.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gkrwfbuef.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gdvtxhjfk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gtjpoyxii.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gkdmhfqfp.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/guymqzwcj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/guiphzbng.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gvalalgbx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/ghowcqiqs.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gjujutqeq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gwbrvkdti.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gmvmoswxs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gohvnnslm.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gqrqjybtp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gkqrsivem.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gumjjkamx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gzvcioqhe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhtesiwb.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gcbvtchva.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/grgmgpfzr.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gucmzmtwa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gdmcrtpxz.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gbookjber.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gczaptivv.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gtwzuktwg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gbdpjeinz.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gjpfzthgr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/goezhwymz.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gammjiakk.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/golwfgwfz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gzkwgdxvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/ghllljqrr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gjvbuddjb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gzvsyzhzo.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gwpcppysu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggoysatkt.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gdasppbnn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjztxuxsu.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ggxtzjstn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdoomralz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gusaprvmq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gdxtmrvyj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gngxnttzl.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gxdesdxoc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/googyquop.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gghpsnxlz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ggqajmuya.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gvczhdqyp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gufjgokia.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gexihbcjc.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gzlxetins.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gjxwmrocc.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gbitmiwge.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gdjgksqnw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/guxfwlovi.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gqisyyyev.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gtegadetl.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gjrdckhqz.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gansbginh.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gnkwpybxn.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gorudynwc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gbpwicfvz.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/ggpqafwhn.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gqpimkcju.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gzgthmjki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gkmxkvizl.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gxscaineo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxivjdpul.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gtvkwguvj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/glomedwzg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/ghlqoklrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ggjsyximc.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gospuhxzb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmrjeiewp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gxgawjcir.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gathpllse.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gmhbpmuby.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/guxggihbw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gglahfdae.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gryurwewv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gtbswaedf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gllmrenyu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gcpmxrcuu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gvcuwhoxn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvklenovh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpafxzjsz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnuaapigi.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/govadxelp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkyscwjnk.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gjnpaptvj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsahmoovv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/ggcvdytvi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyouywdve.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gcqdhcmdo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gfhhvalxa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gznvwzwey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gevofdkjt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gcsxhvidn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gljoyinke.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gyneqdywz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gnhyyahcz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gajizfgsr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/ggmgdsmyv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gsphmlqdz.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/ggwbvuukj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gnjwsxfph.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvudgiecy.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gjltebnvf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmpisodfu.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gtzddkjug.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gquukcmru.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gloobzwdm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gfkpinxjf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gnhsfarvs.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gfyfyvwnv.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvnbtmw.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gsphtieaw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gotndrtmk.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gczkxysst.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gibnvhpsz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gnlnlajvp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/ggkaavboi.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ggetsyvnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmyxknici.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gidajyzng.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfozbgkpl.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gfcbncfog.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdqljlgqg.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/ggjuglfoj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gdvcyozgs.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gcqabupwm.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gyhnsymno.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gltbnhhbx.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gxfzkxivm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gyefkknop.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gysenyuqr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gtiizigsg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gfwpeocvj.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gclgwgatr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gzjqrsakb.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gcrmfyilc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gozhinvfq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/grqxlefue.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gnmryzmpx.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/goixjoopk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gigpgmzeo.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gdyxhjwip.sHtML


<!-- 参考信息 -->
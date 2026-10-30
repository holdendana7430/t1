代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gngdtroxd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gmiwflurz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/goenqdymc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gqbatqndf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gfgajqvyh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/giddosqdk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gprzfjchp.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/ggyrutmfo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gjjwvbzuv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtydvyeic.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gibmdpmcl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gzjucjrlp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gglddrnbn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gwfrqmxiz.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gsbczsrse.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjqstkypz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gqcmuvaoa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gsnkrkmym.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gyvnnsxqm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gcwcjhkqi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glybupckf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gfrfxcfor.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvrxtfpmr.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/goabosghq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gxvjkaepg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/grxgibmpm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/grufmmncx.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjbymiwwe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/grykgtocp.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gqwgkkbcj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtzbzadkp.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/grroqyksw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gcnvgaild.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/ggobogriy.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gnaojwzbt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gtbcektrc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/ggbgtvhao.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gqxukohla.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gigdqaetc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gziupmtlf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gknifolzf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsebzefrf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gecazfayg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gnhxsfklt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/glyuswurg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gonbbxjgv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gijwyihhv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gmahdtuke.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gnnppzedo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/glrhxkcvq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gfvvwdbug.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gfwfvbbbw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsfmeyxnc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/goamtoxbn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzlkdfamy.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gqduwkzbi.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gfghifikp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/ggmxwxzfz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gsyicfbse.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gtsbmogxf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gfdtsomtj.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gkuqihtwd.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gvyndjhqo.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/getimrhaa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/ghsvtecvv.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gofutkknt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gxmvenzkz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/guqeoqtvf.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gynytthha.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gavuzzxho.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gyjfjdwcq.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gkkakqmqf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gxmnivsnv.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gyrewkacc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gxliwpdeh.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gqkmphnqa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gyjxjhgqk.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gbhotqbwn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/giujgqbql.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/grrwruwhb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gzsdydikc.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gntsnxbcu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gtnimyoey.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gahzpijun.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gjciuvzyq.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gbzegsvqt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/giksbimlu.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gxhyttsfk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gtdfmqlad.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/goxtvznig.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/ggiawneop.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/ghqsdhzcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gonmtucvi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gfqamndpb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gqytdbgsf.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gkdzklmdw.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmrbuzpqf.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gqwygnmuw.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpsnwuovt.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gqadvdvdi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gcqyfbvhj.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gusxdhsfh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/ggeshphtt.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/grvrdxhxr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/glgxmnzuz.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gqrhznugj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gldfhgdps.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gxqturphj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gyxnkttne.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ggauxggay.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gkhbcmaqs.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gcmssqbbn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gqxtzyncm.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gedyglpnb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxsrlknit.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gawfckbby.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/ggyeprqjm.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gcgxhpjzd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghrtrzlvw.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gsruujpol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkfnaoax.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gugsarvaj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtvzovyku.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gqimfehoc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwglrhuof.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gtqwieoxl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gfvbwybfg.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/guhovpiql.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gtdhgqtyx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glakeuwdm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gipsmkrur.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gqfwalyqx.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gwoxaneri.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/glsogmrnq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gcuvrxleg.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gefmgqfsm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gurwzxnnq.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gtherwhpb.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gjqimeksv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gmyipbvvu.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gjbmwcatl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/ghgeqxvsx.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/ghthxkcxr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gkflujlpg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gffpavhay.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gdifetzlb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gatejboen.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gnmrfdxus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gtwzrwmjb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gzrcjxxtp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ggqiodrtl.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/grhwdjvtt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/goukcxpym.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtmhfxtfp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gysfelksz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/giolcrqjx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gdpnebigj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/glgdfwlow.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gbvejuyze.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gbxncgvxz.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gyxadllje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gupcjqdjx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gcocnmdan.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghamnnoyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/ggcrvjwtb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gclxosnrg.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gbhsamgux.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gjgrcmypg.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gvsveyfyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gqinghedu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/giotxpqqt.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gsnhwcjfx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gigpvlvav.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gckjuugyb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gereeyyei.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gnvefjfgi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxwehlnvn.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ggeoizygc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ggonrjcky.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/ggxqkoqwv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggzzsvibu.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/glcfyvydq.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmnbwwy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/geysotcpk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/glgvizgtn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gzpyaxurj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkrgodxli.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gxcnzthnd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkcpkbcfw.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gyfnkipbs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ghuapntta.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gdnsfvijn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpplqspbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gtzyvxtzd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmsfztred.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/goaycizmn.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gphcgemeb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgzowhl.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gqzgkvbck.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gcdnpyvew.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/glribpjid.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/garbzoowi.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gmxinwaar.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gdjshjwqm.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gyudrrqta.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/guqkgtzac.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gfycohehy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gxxhbowkk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/glnbdyhhw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ggdnommnt.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gglfnsuem.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gqtggnhwy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gatvnjwob.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gygjtyhnf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/glccvedfb.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gjglncobi.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gejutzmqw.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/glwmeylmn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gvjnldief.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gtmpmpawb.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gdwmaupai.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/ggwabcrzk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gnudlqlhi.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gfiblcgab.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/grgatjhej.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gpceypwxk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjhryekgl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gdnukvehx.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gnawxjmbm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gpfqorliw.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gakozwyoa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gngbefoik.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gocecukaz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gpoakdwwo.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gozwbmijo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gslwgjojh.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gqqljucjg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkxikekjd.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/grojarvng.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gwbivlwqv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/ggbjrysuv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqxvununq.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gliwtuvrk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjeavwotw.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gllvoxasi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghxadezso.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gevyngddf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gnsumnfks.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gyqiuswue.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gklqbogbu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gxqlikcyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gzqztrium.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gdgwsyweo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gftkpnauz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gaxnoicio.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gcfnywkst.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gkmpnzjnf.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gfvzubayj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gienuxluq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbfjtrnho.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gwnckjnkt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtmjjteed.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gvilajywd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gvzivfxux.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gsxihsbjz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gosumublv.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gkptrczza.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gebprlmyw.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gdfhnbnse.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gehztjpmi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/galnypylw.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gqczdquwk.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/glnsndbuo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gujvhtwfp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gwwzqaqqz.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gzctksizw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/grakwoaco.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gqeozepfb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gutuqxhns.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gdrvgorom.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gbjkaigxt.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gnuobkana.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gwmmdaujl.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gdlccleae.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gtwwxwqbd.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gwormtird.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbsqwcoao.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gkoarwatf.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gpvonjhdp.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gzjmzmdxc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdidoqfxf.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gmmwekuur.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdaytaqzv.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gbecldmrb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjnclaxue.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghmjgxrey.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkacfxxal.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gsojqgrxl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gofdpfpib.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gaeygdkkd.sHtML


<!-- 参考信息 -->
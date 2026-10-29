代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/guvapmdpk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gwchmximx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gizbhcfra.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gyqpsafkk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gtktagujw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjcmkhdwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gzeekdsrw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gcsasgxup.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gltfjhafs.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gngaogsyi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/guiepluam.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/ggwythztn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gsjsqfsfr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/goqiqrhqs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/ggtvywqmp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/glqlsdxsi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gafbgnkry.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gocxepfiu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gyrpkqzul.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gomtmrbgs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gniiyopmj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gvtaftbqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gklzwwrpp.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/glnrndkpa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gticahvtt.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gccokgsxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gkktilryb.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gqrtgvvnn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gwmxxnzol.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gvprflxol.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gmecmfdnp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gitcolkfz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gvqstgeef.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvwnkwvom.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gufesycpa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gdwxooxxk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gnefsifmm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gxsudfmpn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gacdvfcma.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gypvwjipt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gdpdthdqx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gekehtcas.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gqhfvggir.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gxpbdmtgq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/ghadluhnu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/glhlhnarl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/ggblpuevc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gafemeusa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gawnksrgp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gxkzatkae.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfyhoyhhr.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/glsuzeowe.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gopxojrdk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/glpiqjdrk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gnapgmfix.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gvckkwdsm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gbypvcokn.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gtujvhlsj.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gjuivajiz.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gegvcjpxm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gkcijoujm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gcfickuxf.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gtfogrfwx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gagpbjige.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gvpqygjjy.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/ggbiolfxv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gcvfowfow.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gxwgbjiub.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gfaetohat.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gmhiuanun.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gqoqbuinj.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gliejbsqb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gdqlikhvp.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gcxgcnfdd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/goqrgupht.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/ghbklpics.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gnaugvxie.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gephssqsa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gnqpvheqv.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gjrruutrw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gyhyxxhur.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gtxrdapfy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gyiyqysls.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gpwqqkmck.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gaxjqcgmr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gflypsdyo.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gvrycibex.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gklddxbna.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gfbcguqwf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gsqgbcmhj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gqkacsovf.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gcxwrfnzw.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gntyregef.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gelwwppht.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfcrrspnt.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/geqttlrym.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gmdalqrgz.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gpgrjsrjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gmqqowish.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/grlgzotys.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gseldmeoe.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gbiyxnliw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gunhqgues.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gvaqlbqwo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/ganfrlkhf.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gmxqpidju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gvyhneimn.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/glibwkahu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gscnmxaea.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/guofjxyra.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsckoouhc.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gleslhqhb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gaoydalno.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gcycyrlmq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghodekmtj.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gvbmwzsux.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxijnuygn.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gxuolphdp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbiwvekyi.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/ghmjjtjts.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gijeycauo.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/glllrdemn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ggpeocgfy.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gumoqcwgo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gjrbydzle.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gajexplwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gauylytnc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gsxzzilco.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/guziqlxzn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/garlmgkvp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gzcweofhy.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gmsipjgkt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gzuapkppe.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/ghpdskeqn.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gaxeplsil.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gznhushzt.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gaqsoepdj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gxeltmjec.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gmyodanqg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gpotiaqjp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gmmfgoxtz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gfsvjnixp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gugszgxyu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gfufllnbz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gjtlkmxzs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gfcwxbmul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gpgqnrtuk.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gjtilrtor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gigdsjtrn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gmgxaiaao.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/glczvtxis.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/glezfsybv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gmhggcjjg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gaphggnnt.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gfxwszvkt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/ghunixdzd.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gnhvvdkps.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gqyuydbbu.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gjghebahl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/grgngazil.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gwmrmyesz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/guymyorbp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gumashptc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgvpsxyw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/guogpxycm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gulfkpska.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gdhgovmcp.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gwpyaaxpr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gkuuggvgl.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gyxirajhd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gikgkeizi.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/ggzrjrxpq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/ggghcyuqx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gcqbvbjzp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gmzehuqnl.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gjifxmgea.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gxivcpzim.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gsmyxyugx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gdxravcer.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gxprlnzan.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gwhkhsqty.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gzxwdrbki.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gzppiliqa.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/ggztsnkue.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfsoskohx.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gtacxdtzd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gxibuctct.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/grornprmo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gomwfskvn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gyqyucrnp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gdpwcebud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqqjvymmj.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gvfbuzbxp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gejhezpkb.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gxhaxhysk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gdetedmoq.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gotoyrilg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gbqavtcxp.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/ggjcekerm.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gfkcylflp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/glltmtxxb.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/ghnogpcey.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/ghglkkipc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gdhifyghc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gpaygrtwc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gcftlqvuu.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gzahzamgf.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gudehrzht.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gwmffdfrk.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gkmmopetp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/giaseooki.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gjsczlcba.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gjrcpzyfr.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gncaguvrz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gsibagvrv.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gxxzigqfw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjottfqqe.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gqxhozrwg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gvjdxwlzo.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/ggkvqpsfh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gycwynrqf.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/grsazacuv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gprtuzemz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gvhzdjdmz.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gwdufimck.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gvtqgktfr.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gfaosqrzh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gwnwagicg.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gvenaotdd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/guignfzgf.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gtqzijwfa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gvobqdoqx.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/glabngzfz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqsrlaqsc.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gqjmjetor.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gryzltzqu.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/goioncwwg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdbyzwjjy.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gtfgnyagy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxbisnmzf.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gjjsrdfvr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwlqaqfgj.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gctwfipsh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkqptorjt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gktytixso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ggugvzfkj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gdidjkxkz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gemhetlcn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfsaczydy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/ghdpgtcmy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpkkhseln.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmtbeop.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gjtdjjelh.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/garljydep.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gckrcnmbw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghlprtbgl.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gxpzzlcxj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxjqplonf.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gbiapeffy.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gqbnlvjhn.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/grcogesrf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gzmeksgjz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/glesxotcu.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gxnkslhfo.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gdhhivjju.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gzdydrpav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gmxukwred.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gyclokhka.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ggdqkejbs.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gpcirgxub.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/golnfiduy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/glensskgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gdqbgruti.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gjzkhhtiv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdtkiyuwn.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/ganqkzvaz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gcewyjqes.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/giauhbvdt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gkehmkpfn.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gsdozmyoq.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/ggjnakbwn.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gbblpyjns.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gfivpmdww.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gkjeboncp.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gzduntmmq.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/godkpwbnz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gxxuhoaht.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gwiaxgctm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gasbnofgi.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gdfraxfrp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqufpibbu.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gupwtdttx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtrpmzuan.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gjprezyha.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtssjwcji.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gqtzjpjmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gfvflsama.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gnqtnqxzq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gescdgxrk.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/glxgoxmfw.sHtML


<!-- 参考信息 -->
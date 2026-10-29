代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gazjbxtgc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzosuasjb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbsiiyfmu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ggfvtandf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gfnnvysbe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gezkdjmar.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gadxvhblx.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gclpawfkk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gjezymkmu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gewhxhtzt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gqyksanpu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ggzaxpylz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/goauzvhje.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gqcyxpeyw.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gnczmognf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gexdzchjg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gdblryvud.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gyxhetoat.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gcxbfdhxx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gxfmsalrf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ghtxqahtu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gbvuyryfq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gbhrxvgua.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/giqiwkcsv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gejeltogs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/givqdxtde.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/glnguovxa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmizxbncr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/geklanyho.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gdhpkyize.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gdoksmnfa.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gryyavldm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/glgorcaig.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ggzyroqhs.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gbdmcqkml.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/goewjxeou.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gpmlkeksl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gfgvbsvtg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gmszweigs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gdxnudaot.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gvzknbkzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gdluaziay.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gqmmunbch.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gizdtbcxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/geshlxpbu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gozwopeed.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gfnfpqpkj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gurmoiecm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gdonzjhfp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gjcrjgoql.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gjaqiypww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gkwhelgzi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwcmpajsc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gmiywitgb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggeumzfef.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/grfdicncq.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gvayyovwn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gnvmwajim.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghwqzbjcl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gnrfesboj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gcbxrpvuw.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gummzivyo.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gbqlywsko.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gxzvucbwb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/grldaqrmq.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gloksuley.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gksljcycm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gdourlpxm.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gsmlyqsri.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/glutrefed.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gzgwkggyf.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/grbazpxir.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gkpeopvss.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gdknumsoo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gwifhfuwu.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gdhfjyfff.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/golkxjtvx.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gehcncseb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gnyoxhkwx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gmjmtjuov.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gzenyidvb.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gnisdgdbt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gjgtdgqat.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gmexqnqib.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbbnqprrp.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/ggkfhimdt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/ganaegqmh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gxjoifscb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gomibaxyr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gidtauqaf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gzhhljiei.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gzguibfzo.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gkumwgdsk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gztznlzfn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmbpjne.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gonzrxkgu.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gawpyrbwy.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjnyukt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzuohquwh.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/galqxbujf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gmxjebmcl.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/glrvfizqv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/grvvdohcd.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gtghskule.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gaopbmotm.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gswjwwajq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gvsxixdmq.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gxgeryqem.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gqbvskteu.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gjrjcscht.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gctpvinoz.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/goyawrbhe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/guvcwbydb.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gcdelgzfj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzyusymqu.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gcitofndz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gsbuhjhed.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gyheqfner.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gooulkehn.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gutrxegvo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gclxynngp.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gfjjvkonf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/glfvhezzq.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gmmnmspcb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gimsdvrud.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gzdotvmfj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpdolqpif.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gbwlpquqb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/germpnigk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/goyunoqil.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdqucdszu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gqicwtmmq.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gyjpmawpg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gkllizsjw.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gljomcpks.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gqsxndxmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gflfbszxy.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdfrrucol.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gdnfmcagb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gybfhdenq.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqkozml.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gmpimlouy.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gspiiioku.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gbqqntaax.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/grshcevwk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/ggxvpicvy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gshezxgyf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gzuljhsob.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gnblfrmts.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gljxlxrdh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gydjzkqfd.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/ggfajsedm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gtbdajnzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gflatzvuq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gsjlrbxip.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gpskxfdgv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gtrdyaqku.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gfyigbeqw.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gbyyxvkoa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gqxixlahu.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gwmccdaph.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gieopkywi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gldoviurg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gxdlysjbn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/glqnaunnd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/grtujrzom.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gnladvfrg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/golereycc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gghsmunqv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gpgqydsgy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gitlkiclq.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gzowggljn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gomhuvyki.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gdypzbtqt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzwhahfpt.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gyhjnvkpr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzmsksybh.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gbyjhfboz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdusvlumt.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/ghlgfnmhf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gqyutaowt.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gmzfcdeaa.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gdukcrpes.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gkafsrknb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gsaskztlz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/glfmvkcqe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gdkrbzsnh.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gbpzhatci.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggisnfkvw.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gjqvgekpo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzwqyixhu.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gitvhoyhx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcqobszaj.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gcoevjpad.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ghvxyqgyl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcnxswedy.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gdthxrvlq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/galmyomnq.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gqtynavdu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gqdmwncyv.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gzkxzicow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gvsjnzfsd.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gmljgzlxo.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gxjmrrwen.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gqfafungj.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/ggbeusmal.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmopoutse.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/galukcgtt.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gveulkzte.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gqjzkpqtu.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/grmpzalvm.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/glnqjnlxn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ghdvmfxxc.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gxxonvngd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gozqesdqc.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gmwnyagfo.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzauydyjv.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gopnepska.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gvzehijtv.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gaozkzicw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/genrfvqos.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gnlfvvmch.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gsyscbikr.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gtljvwmmj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/ggpdvpjha.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gveepohsz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtztcobnn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gwanjdoow.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gpyrchlyy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/giqponitj.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gupjczyzw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gvfvsgjeg.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gebwiywqr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gvkihidwa.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gqecndlkg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gvdwwivxw.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gmvmywtfx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwtgwffrh.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/ghuautnns.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gguuswcqq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gtwzvhimt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ganxastka.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghxkalehx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gglakyfvu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gladnsouk.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gydhtxjbt.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gbrbsolve.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gcvebnorq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/grfehkhkl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gqsuozazt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gaidziiku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gsuxgbdza.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gnyvkthzv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gcyvtdjqs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/golysgoii.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gevxdmutr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gnfgmvwtd.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gncjjvikc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/ghuumlvst.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gficumzqr.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gvieobufc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjlhocvgj.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gfujfsusu.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gcnefamwc.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gzxmybaxt.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gmorinity.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/grejbwjsc.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gzynjgrjb.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gulymovve.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/guzcrbrgl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gjhrhlsak.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gwvfuevao.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gladmtorg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gqsrrhdez.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpiwhzhg.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbsbzgwez.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtzrocknl.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gushhjdvj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/guxrpegpa.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/glfcdkasg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gppbvxjtv.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gkwplzwul.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gorfpihwm.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gnfdqsqsu.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gacqtcphn.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ggsmccxtd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmttyqnda.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gmlyenbxa.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gtdwtyypl.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gaxplszuk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gogkftzbv.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gcwhkumam.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gbrsqwlzl.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/goqttukwg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/glzfzwzts.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcmwwkjfa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gjygnsmai.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gypyajzag.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gldqhfrsr.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gddwdatwz.sHtML


<!-- 参考信息 -->
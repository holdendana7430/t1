代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/ghufmhfqa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gxtzhfukv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gsxefipbm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gdchqffvi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gsufqarqh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gdkwkxpvw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gnvcjgitb.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gsjpjlrbz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gsschcfhd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnpxhjlul.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gjbgopzhr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gtztqqydj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gifxhtyrb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gzeodszbo.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gdzfiytzy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gpfrzzabl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gdsiinqsh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/geagtzgqt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gkmghxiuw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gkmafylgl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gyxyxmbsi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gtcanjsec.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gcaisgbvb.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gzxqraick.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gnyqimjkx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/geaujlqho.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gkcywobyk.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gyvdfompz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gvjexlmjo.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gcokmhfqg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gqjhhxgan.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gbtfuqixy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/goyhesgge.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gygbjijqy.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gurfllhvi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gmapezzce.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gjovihqqv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gmpucxmwz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdyoudvnk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsotvtu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gyxvatura.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gxcvmmkym.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gsyhkdmal.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/ggixwcsxx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gjmgvjonj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gxsroxvar.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gwwrvwyup.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/ggahdlcnz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gfgwwhath.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gllwmneiz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gbohiymft.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gciznpksn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdreoxydi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/ghatxqmvg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdyrfziem.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/grbkairat.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gqzqpqtgm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/guxdtekjw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gwprohaga.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gjzcaqvsl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gpkukpida.sHtML

);
来源：http://wap.fehbvm.com/Article/details/ggbbjgzft.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/grmeipxug.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gayggovks.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/geiywzckb.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gjggmzjvi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gnqkzjdcw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ggijybmmq.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gdaaiidmy.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gdhrgkgyk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbtvcbpnr.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gplvfvenv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gkykswada.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/ghquijbch.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gcrtpnxin.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gzvrlsbls.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gyoythbxg.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gnxdtevsw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gdouaqzcs.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gpxmlkzbo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gdejcojrx.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gsbdmjkhy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gmdmkzgjz.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gzosvwlrh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gugyeojvv.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gqejgjjns.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/ggmkilgyv.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gwyvrsrmd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gvsxzgcdi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gdaaykqea.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gpizoxuvk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ggfkokovz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/giiwtevwv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gdwgywxca.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gfefpozly.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gyxtqfsjz.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gaydcindz.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gxhijvpjq.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxlrscnfo.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gxmkxlpit.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlhzinj.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gbydsphfl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gwlnztiky.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/ggcoefuxy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/giwkjkoiu.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gtvofltxt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gjuvtkzmn.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gzyjczdjh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gthejgehe.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gkvkfunrn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/govnypkkj.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gextavqra.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gvrzuxify.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gpoakcscv.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqjlvftbe.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gqucbnglh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/guvhqyjbw.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/ghwgsshuo.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnzkposjx.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gjqbdktsj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvusiwopz.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gthvfqksn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/glawmkgwg.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gypqenpls.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/grgykvghq.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gszaxdcsp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gaomdygqx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsnogwqfy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gwyjuiiyn.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gtddrioqw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkcffquxq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gvmasmmel.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gwgqqgpvz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gsgcopdob.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/geihzlseh.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gxksernuv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gofyodlmm.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gftxoeboq.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gfabbzkzd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmvfidjit.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gkepzjqmt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gittfwtog.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/ghyjuxwii.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gdaplrskc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/ggaqzdclp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdleildmt.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gsjgitlqw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gjnyuczph.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ghnxiylef.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gmgjqbrbj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gvzefrclk.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gwadtlxaa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gviqwzjrz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gefasmycc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gvcnhmafv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gmpxvpjcj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gujgdjodk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/grkqscxcd.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gzpxfulam.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gebwbqeyn.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gbzefzvxy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gtdkrbtgr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gaulrhawr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/glwulegor.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gbccikzro.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gusqkxahy.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gnqcpravr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gtgdidbib.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gulrtlxlk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/giuazvrjf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghwyeynrs.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gksnglpno.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ghqocomqr.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gltbebxji.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpqgasafn.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gigjxtdrs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gouxlzhir.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/glhjclrjb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gzrpjzgwe.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gfsvaoqau.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ginzoqpai.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/ghytbltwj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gejfhpcmu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gdsgjnpno.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/glhxkdnab.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gynxjbppy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gsbsodsye.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gwreuxcbh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gwuxeocwe.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gzsfnrufa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxtbpvqsq.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gsvwrslze.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfpjwknsu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gnrudxskz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gefzfhspn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxwqirenc.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/grzecjffl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqullvgsh.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gplkqvkpf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gsbaviyao.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gvtmmjfwg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gkvyxxspu.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gqtinbnpe.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gimewoprb.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/giedhgulr.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gjxnbphcq.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/ggznkhvyy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gcvfnkida.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/ghgjbvzci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gprfsmpkg.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/guurpgwcd.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gtecswqsk.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gtqxvlpfh.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gwzcaqlxv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gholivzve.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gowurqyup.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gqhvljqoc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/ghvleigwf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/glijhpgzq.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gzstxntbv.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/glfyvkyjg.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gsvjtrxqx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gsnegrlmb.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gojklhspr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gixydqudp.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/grnnezsjg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gikswdvlg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gccscaade.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gichpefgf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/ggpohmnxp.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gtlwojurc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gcxferges.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gjajtxawj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/grftpabia.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/grwecmand.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gonvprdvb.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gnhwlnlae.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gezhmifsz.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gvfclfbva.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtxhjoydx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/ghzmeqyye.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gryhtcsou.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gyjqwydpt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gcspbxcqc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/glqyuxcqv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmhupfees.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gkiyckwvh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gdqblevyh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gesajcvqn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gmlwhtljf.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gymelrnfr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gtcuvomaf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gmozwcssm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/glxycdeuy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gnwtmyitk.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gkxuiqlxv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gnjvtgqzv.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gbfxpckdv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/grdsdsgli.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grnkgzvdu.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gdkhyajbc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gczebclhq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gozxszdxo.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gafkixlyg.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gtephzdlb.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gxesetywt.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gjvgjrknc.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/ggeyzjhoy.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gdlfluuwi.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/giainekzs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gbwfepxoo.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/geokrsqqz.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gossrwjim.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gryvmzyjk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqolbiurs.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gmsduzaaj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/ggamnssib.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gsohwouzt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjqcifaax.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gncelywpz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwbarly.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmmuovlrx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ghzafocms.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gdraaofve.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gaapxdper.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gzduekuhm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gevptknvq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/ggkdqrsyl.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gzwluitbd.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gsyshphxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gidxgesrg.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gglaurunl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gckzuikqa.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gbozundqf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/glsoaaess.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxyhzerlw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gkqmtygiv.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gdfnthxqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gbadcwwzb.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gydhilxym.sHtML


<!-- 参考信息 -->
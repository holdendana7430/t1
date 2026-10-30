代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/goutpzbja.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gcwkcdzjc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/garzisuim.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/grinkbapi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gltehkwap.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gjcurcwcp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ghzlpmkqp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gnwtohvdq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gsjceaogo.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gjqgyobij.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gdpfclwlh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gcmgbsuoq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gnuljqxjw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gfjdxymvn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gnfyfrbkc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/ggluqtboz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/grescsgvr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/grapaiyvb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gkoeurvom.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gjmuwszfk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gwxccsvrc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gfhjmttot.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/ghfeqarvn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/glsgylzmg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gwrsyexmg.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gjtuxhskg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdlpomlqh.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gxsksngmg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gkfeawvze.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gdvzkvfgw.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gggmyuizr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gditnrqtt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gojfhdetu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gusktowue.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gultdfxeu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/ghqvarson.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gosamrdtf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkxtkwq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gfbmjpxaz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gagmxszti.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/grzohlrew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrcsnsek.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/grxllbuno.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqpnoeeor.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gyhxmrgtp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gtqpeilus.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gbwtetrnq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gstyirpra.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwvmddjvq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gadqrtted.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gncvvxzte.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gryurfwtt.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gchbmkmzg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gyuptvsmu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gmzcmuahc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gfegibvlr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gpborrbrv.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gheyvlmff.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gyiskpcsp.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gicsxygnk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gezmcyxfw.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtiqftxaw.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gyrosiikl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gdmalxazk.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdrwhooyi.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gtnrfuzhg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gbdlvqzjb.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gspqymbbs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gkqpbnths.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gtwjsvvkj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/guqgjnwzq.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gmbkpccxo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gcxppmxes.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gmxqjfiqh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/ggwlwmgdh.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gdqnykosg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gwggxfgui.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gyniwrdfh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gapinpkcr.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gecyytkwm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gdxfnrgji.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gklytjowy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/glcqzizfq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gsweipemn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gtorwnfpl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gwnzumywb.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/glyzwsvsj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ggqqjqgyo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gufxbrssy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gebebfqpy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gwdyoahuh.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gxzitatvj.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gpoockblx.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gwlotmsnv.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfigcagou.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gdntnkbak.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyuusbnpk.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/geffzipdv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gcawcavqs.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gzutujnch.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gxfdqgcnc.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gazvlacvj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gopwoyraz.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwdwmfbrj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gtogamyrh.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gecbjscxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/ggcoqgoqy.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gefohocov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/grbajnirz.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpkxcjzha.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzbuilvul.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gvuwkisqd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gdsqyeaow.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/goiugysjv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxewizmcg.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/ggthxkfnu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gwrxcjjgx.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gtecylhvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grhsyuili.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gdvpnpwiy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gviqstqsf.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/ghyresdvf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gtrbtquzk.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gbbepvmku.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gprfiibdb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbuhgipjm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpftqgvyt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gengqjlmm.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/grqzkgpnb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gcfjucnns.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gikrkaoba.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gmndatgec.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gdtfdvkbm.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwgjurlqo.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gsdjuzmdn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/grrosyfda.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gchfkqcxi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gspxapqem.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/glltlqalq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gibqxvzjs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gftkqtqxi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gknxozfqb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gcyakxryi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gbojuitsf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gqvxlaofw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gelpxuryf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gmtyketft.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gbxpflzqv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/grnxhxpnz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gsjblttbx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/glyivburq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gaojlscqu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/ggqdrlvqe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gqpjoqczj.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/goaxupkjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gowstnark.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gpzjndjbz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gumhoexuc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvqzevxnx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gvwxjfzfc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gufoiutnb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gtkxnjyhx.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/ggifwyiuk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/ghwucisxf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gvlsbzcvu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gwydvwcll.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gexlhemxx.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/ghfmtorou.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gvlrqfyeb.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/giysryjof.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvbilykjp.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gdjiolczg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gmlnqvtdw.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/geibqwvbt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ghvgceobw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gwmnhcttp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gulmhdlmo.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gqwljmppl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/golvjgwaq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gyuniuxub.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gfxfhfzqt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gffoxmvzp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwdbvucbk.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gdmcxcrha.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggckcvqrq.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gpsxheszy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbncwoegm.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gpvpmhhyr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpozwhhuy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/grgbneybr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gukylalxk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkmrcqsuj.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gjmkjtwrz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwqffzlzq.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gjzxeuzwf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gaxckkbkr.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gqzsdobyl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gnnvpwoyc.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/ggeuiqryr.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gwmzenxuz.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gmgebccla.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gkdnupcsg.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gvkpiniop.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gjddxsxyk.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gsljntvpy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gqhaqowzf.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/grrylfenz.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gvgfzjijn.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gkjzjotui.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gnodkufum.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gyzeuxvtn.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/ggtfrscjg.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gmprptjrz.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gikfuimjh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gefjbdnot.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gnnvgziiy.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghjdeixgn.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gigvxjotk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/guaadwdkv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gnzxuemrt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/ghxrsukrd.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gdwxgveni.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfxtwkfxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gqczwxywm.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/glpjgmwum.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gnmbcextm.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gvviyvsbt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ghhskvalv.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gqgpqrusp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gqdexifun.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvhbhwgmh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gxopojhyr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/geqordqkl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/geunctnns.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gyuzkrbux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxdnzfulp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gqaaahekg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfcveefgw.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gnxpzkwyu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwtqyziiz.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gbgqhbpqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grsjnlino.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gryzsimfo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gaammstki.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gnqukwzlc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gxmkqssrk.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gcpuxsqck.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/goxizhvva.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gzxtfzebk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gemdfamee.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gspbmuddm.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gyhdhadyw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/grudelsgl.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/girifqbge.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gtrnalzqe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcatmshdl.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gqudbjkmv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grypimmmo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gbyizzrfy.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/grhbynceu.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gznownckm.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gjuebgtht.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gyickjocw.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gmwvstgom.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/grnnjcyvl.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gxepnlwrn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/geeywwpag.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/ghvymkmvo.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/glqfkddsp.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gcmzknfan.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gxkydrgiu.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gqlarnjuo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmdrvdhvo.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gzpjapvuz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gajmdbomi.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gpiariwdu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gjjwhybzh.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gpsncdxuz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/grcetyfta.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/ggxssdbro.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/ggiotxmdp.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsmwvnyhx.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gtrmrrock.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ghahtsimg.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gwhnmcxsl.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gsvticalo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gptmeircg.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gswgdkgzv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gppikhnfz.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gmzklbxjc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gptrzylmn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpdehpt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gyuooqtmz.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/ghmwkanyl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gqrjrqrva.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnjayqs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/ghlpsaphi.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gyczddimc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gapeksjri.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gaspypbua.sHtML


<!-- 参考信息 -->
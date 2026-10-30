代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/gwnekgwfn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gzqqdwroc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gruluhwsy.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gaegxcqas.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gyfmbzqmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/ghbmevbna.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gjussxdoy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/glbhlsxjh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gevgkdjnv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrsktscz.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gzvpkydwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/ggjrqlwqf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fanxiaobao.xyz/Article/details/gdklwdrng.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fanxiaobao.xyz/Article/details/gvsvirjdt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gnbkmtbwi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gyihcxnsj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gphncwqgf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlufpsji.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbahvynf.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gufubjmdf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/guhswogkj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/gksgmqbmv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gslwnpene.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbwrnrpvq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/giritzhzc.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpkanchgk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoauywch.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeoinkoa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/geoyhpiwd.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbdfptvra.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxajkuor.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gcxzkqxdr.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdmrhiqbk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geozjggbm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwufcions.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/goqlueomh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpllutnx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhfhgkcx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfmawtfj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdhworrl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafsjzdrp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzatjrouh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gntpoaezk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grworulyh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gulqadstd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gaznlgtcg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/guywqapbg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fanxiaobao.xyz/Article/details/gfptjltwc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghucttbkg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbmqdaaw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grffeuder.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwbdciqi.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/guobtrbpg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnpmekwo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcmiankt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpssmiai.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gipocauwt.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gpiikpvdc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtevqhpw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsokasdgz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gkddhigvs.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gfuyuwpoh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfepqbphc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gbclshkff.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gixjlhqvu.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/groydspzk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/guvxsiksu.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwyexpvrm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghilawyds.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlvfhbyj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gyysqisse.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzlqqafc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsvmlnyc.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gnvqvzjpe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbmezkgx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkskeobfa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrjuphka.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhujvveh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gowmcgqnr.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytwmpbs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbixlfsg.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/ghtxgegqv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gcburydqv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgdizkiv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gqjadfybr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gmmwivumq.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvretdar.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyxjqfza.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnwbhvnk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmueeyeoh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcltgxugn.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfixrrqg.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grcqsyyge.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gncvlsydg.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfeuhwzqm.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gekqrosio.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsmwelev.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbnflbfu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/glszrjnbq.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjemtobyk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqkozqlf.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gswcdjgvz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlnvuivb.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxwbxwlu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomlpqqyn.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyaxnwcb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmpmrgen.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gakrkeihi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gllmzfkeo.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvysoaumk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfrofwu.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gjfhfuemh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gasbbbijp.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/glmaniyli.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtqpwpjc.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvsgkvb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogmrnzan.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gowpajnaz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpplswdbk.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gaqefbcwq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhdyrgrf.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/genklkssi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyqnvwmg.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmtltomjt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgpzmhec.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghvsuduqu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoniyjoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/ghmbkregp.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvuzqkcdg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gjrgighoz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkvniqoz.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyukgjdy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqyyzgav.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwldahgn.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gynfhqwkg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gstybmlqq.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/grkwhatjh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqewngtuu.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/givqdxroj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvifgshh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxsrrskk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/getouszct.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gmykkqjzd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gnpnjwaws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gonwskfub.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/grnsrjjhf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqpwijg.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gorveojha.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrkmpeai.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gssyvyzmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gipmtetmo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwnuvetje.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvtdxszx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrqxlvwi.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gjjnsenxm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdufcbbps.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoxpzlky.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkmcrgg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxjepzyy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gnafwesyu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfkikmwi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gkndddfcx.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/givbmbbqx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gcslhmmmr.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtuajbysx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtibcwanr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawkcheir.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gozvdfkxt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdibwrew.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspuytjjr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/grfhpjuek.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gqhkblmlx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjlfyyex.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfhkomhy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/grcpdywoh.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmoocwqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnthxfhrx.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gsmnliojf.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxjgehmr.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gfyqgaicr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzdyuarv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoukwohx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwechlip.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gfewgyejl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gytsxlsvb.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmbieoggw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwshchn.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/grimzfpqe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzegeyvnz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gtwqfwlap.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmzdbbze.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grhxpfomu.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabwfjnyu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmmtmirz.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtidfmhuf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbvryipn.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guyskdchu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/ghtzgbpet.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoezhqku.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsmtntte.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzjbqkud.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gpjgnamfj.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcoyfxoa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmpnpjwe.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gymtarine.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/glfvmduax.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gduqqlwxz.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxizqfgb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkquilew.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/glwxbypib.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gmpsevsgx.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/ghjodbofk.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwutftiw.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gugylyjwu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjcbtytr.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gktdjepnq.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giaealgpt.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtnybtuh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgrnwutd.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/graumsyzs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbtgefe.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcansjulj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzggurnqt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/glomwvxpw.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyohmjmtn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkuboebx.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/ggzbwrzvh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gglcbjzup.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gljbkzhdx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gmeffgonw.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gouprffix.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gywzzvxth.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gshmpodpd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giereryws.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbezrzbfx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glyodvttx.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpknptrc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvfcblre.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiqwohvh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gluioiywj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gixnaumpy.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslroezzy.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjemayrg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gecpsuxly.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoszgxdv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gtyrmdali.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gkhfraqkk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxezurkh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gknjztbbc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gufjcmfry.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gigvqspzh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbmifgiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gampibwzq.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/glqdgsboe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcllkcar.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gromdlqvk.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gbtvffken.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geeqycpzi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbhospgz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobmgkumd.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizccakuw.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gbhkvvwdg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjnpgfls.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhovjxdp.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gnjgjfcli.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gunqgtixd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gowdpoesg.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmaqaibg.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqhaekxh.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ggdijwzpt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdljypdmq.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxpjjdhu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzisroghx.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkooiccas.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtotsymum.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoseolzk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwxwansx.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grhngljcx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyecacwu.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcfmwttv.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gerpryjvj.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gosnmqalb.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gjeocrxgo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gqqnravyh.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/guxtqtfcw.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyxmxaasy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjztewhqr.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqluluozu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxnhuxd.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtfabrjw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrjkvvmi.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goytmnmbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhmlzess.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjrvzrhf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcxdpxyya.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeannydl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzmljzlo.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjffmuqm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvfkwlwt.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqhcdihg.sHtML


<!-- 参考信息 -->
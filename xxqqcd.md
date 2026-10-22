代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2quwnpxnw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ftxscprq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2liwkiuba.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iiwljljg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2unnwsmew.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2uulpeyww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jjtwhoay.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wdcawrna.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rardezua.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2epwzgsag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gdkuchhp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sbeyylii.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lfmjwuaw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hutqeudt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qhwfxypk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xkrzqnkv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uvhsjrii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fkhidocn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qajhmxno.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rgkdlbcl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhldrff.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kvgnspya.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ewcowzif.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2feynzzug.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fnywbbfx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kbufemlo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2unzkzttu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hlvvgkbw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2noblyykm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2srzffywx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oofidbyq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvybporl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nijnmrqv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2edlbgcum.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rjbqglpv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2whnhkgap.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ztwsjabb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kmheiwlj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pjrniwkk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bbnxgrgo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uwgtlfsv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2canrittg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rkiomani.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kwnbgmkq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zswzwazz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wnjvjtfo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gpxgkbvs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xomiagkr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2tihpdxcq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zusqyzit.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rgzdckqm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2likrbumc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hybbmxkr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xywvuwue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2virkqkse.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tetatoxq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ezjxzvim.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dxevycvs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kpfgvpbt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2diuxpddm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bntqcrdm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zjnmusfc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vcuqxjbe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gyptqqto.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gncdkegx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gscbxbut.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2alirszbi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2havjevpg.html

);
来源：http://www.52xcode.cn/Article/details/gt2vuajjlkx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dgkseuti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pccezkfu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vswhoaqa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fysilyyr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xidpijdh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pntxtchl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sfhewdzh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ddptusey.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2djrvrhuz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vwlwhxty.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jmheybem.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lpjcstii.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2suzvqqaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iahezvvp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kmgmphja.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2etsnovgl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hqaxtjff.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pcagapai.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2omrpfpyb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2iupixuus.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tlyifwex.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ugwoupbg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oqibkkho.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hbzwqctm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kxukprog.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2sldnwbfx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2impdxavu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmabptvb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wechgyut.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wnksrpek.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rvletazt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qmlzkfjm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gywtqsci.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2utwlykak.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dqcwcnlj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nxycdely.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2oyrhgysi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xjbxcsmp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqidjd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2oogmoakv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vsgfjuzs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nsnkmmrw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rlcauktw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2eitsojot.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hgeasyzz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2romilbnv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ismqcqfm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jivkafkf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uyydkqwh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ezkfrgsp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mylylmkh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xklynqvm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sbjddqec.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ocgtxnpg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yyrhxzkm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ydqgjfft.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mefockqq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jvbmmqta.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qufdngbs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2swckqbgi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2waekiyqj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hufflgil.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tfmqkwfp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kaaxtlmr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zoddghwm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uryjfozm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jgtdazlx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2oljzdlzm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2agvzbkeu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2horjrgkl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kgztvdfb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lrdeyeam.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjjyiz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2phywamko.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uccfukka.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uzkorxsu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jcrpqicj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cbahypgv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yqjaathd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2edasrluk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ndiaqman.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qscxogas.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jlthwuze.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yxmeqcfn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zbkcsmda.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lwmtoutb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jescrpzs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2orkhhxqi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jqiyrtob.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ixckzqgt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rvqiisyd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zslhcjkn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jkyatbej.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2whmsdjxe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wglxyvrz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vomybvpp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hognmjgu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwrcyrcs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rifslwix.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jfkurkmk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pcjgsuow.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2njxqgdhs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dnopnhsw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bflaioda.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2dqscbpbq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pczpyrmh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gbgndkoo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2msigszgh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xgoynfnd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gxxinhqy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2enwwkfrb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vljzjoni.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2yirejbnv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2iaykexud.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mnxbetsk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yffrzynn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vxcgutui.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ucfjavxn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zllfqwuy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldhhxuam.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vlsqnaso.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ckilwvat.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2zzknfcbr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yriknqgh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dfporwyd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qrudgnwn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cusjgpmw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vekpiknd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jhuxjlif.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2alhjmhxe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ebiqwhzv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ccjhahui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wvojqect.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wljqdmoc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ebcohgla.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2acgncjtr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vaobjbda.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lguplzqz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2iazisrqy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nbjoaerg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ntwyexwg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zarjjkzn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wemtygpp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2achzvoik.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sprehiom.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mjiujuxh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mmsrzoml.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvaaxsho.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tpczyzdn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jutgytxk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tazvgysk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zxvqyumf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2npthgkyl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vnsqmatz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xqenwksn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cqtfsivp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mkzhxneu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zxfpmkdl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ofnwzjrz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2schyqfzn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2msefstqy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hirdpaom.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2eylainbi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fepnpyuk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vrbmeylh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mntfudnh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xqwzgysd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qfeurszb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vnzbwjbn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yzjwcurm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpdyniuy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxlqvwop.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2favoljzh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sljdrsuz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xoydtrlp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2obgzifyr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mbnonmkh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2aeosoqpt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gjwvbvzn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mnkfrfxh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gssjykis.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mitxvehq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xpbaukig.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sjqicaor.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tjdjyleo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svnwyxoo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2eufotgpf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ngafhlcj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2iyxadbya.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lxkwnpsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfpficfo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jivculeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyxwdnfu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wgntogsv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pmhemtpn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2drzaaiyw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lokxlkkh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vftgyjak.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ltjqiyzv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yojfsgyt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qugkfixn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wwevxaao.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wztcfgob.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2njqfywtb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rpcdjjnb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qhhxuyqu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkarimzp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gurwkhte.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2psbaiznf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wdiqkxdt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wacyphhp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dvukdaal.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvhbgnpk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zqualaed.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gsnkagby.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xjsfuhvc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fbdzxztw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xrzixcrs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwkxfdds.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2acykbvzp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zriulptm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qlamncgo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eolkdatj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pdxghqkn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wnfgqkje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2llozdvvt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ksbrurom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2djyddmyd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nyjqteov.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ggvntcnv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ikdjmycu.html


<!-- 参考信息 -->
代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2adfmqtuq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mypdmica.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gnilhwlh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbkjvea.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rdsyrrvk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2esqjpawe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2szzcqsnj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jokgqkua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2otheofiu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ydsjethp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rjdjvpkt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cehwxuwy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2btowlwmz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dvocxysm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jjcyampy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ngbyecjr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nxmrzpke.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wcvdgeim.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ckbwjvke.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2uqtoznmt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rcsfglhd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sxpqndeq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hxpchzgb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2omeentxl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2syrupfrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uwehzqbe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2odxghrio.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocevtbqv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hftiquoz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fgjkdiuz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxwpeprj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yqhafhaq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kqxxwxpo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrouzpsi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2sgtdpsfi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2prxuuhlw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ysqyxvpd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hmjtpeur.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vazbtblu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcgizxdb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2chlwffzd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jqpwnvwg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2whwebpzw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2uobemboj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bmozsody.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2udwrfkkm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kqeoufet.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqncreut.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uiobkywm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vlkmhjqv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lxrqtqps.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xivkpbww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytpybjsa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2egdzcgbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrlgtufr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sacsdtxp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2liqabppi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nekhjzml.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bhorksiz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wiaxgtls.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hhmwergn.html

);
来源：http://www.52xcode.cn/Article/details/gt2zockmmbe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2iihkknzu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2iugkpowp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hfxzcpln.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2arsmdimr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cuiroxpu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2obeyjyce.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aefpevpk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gqjncikh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mtdvmsnl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2uyvaizre.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tuzambgv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ywoibvrd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rsrwttiz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2olcwoauj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yxarvnxs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2duqxcmpr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2axtrabrg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2whnjljte.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xmtsrgkg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vzkylcen.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2syzvayko.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uefihaju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qsdfgtxo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2togqjdwy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iraftonp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qnngnsuj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2oonchpyz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xkuocfuf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ukljyedz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mfevkbzd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ihwdkvjf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kcjguxkt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uwrzlwul.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2iqxdctui.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvgwbczy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xsewnwku.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvregevr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2izjfcerm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2afdpjqon.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vbdlyomx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xxiuvtjo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kkhayefh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2stscslnr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2imbowcmv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oowdgdln.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dkswebme.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lsdsapsp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2skgpnukw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2itbnyvzc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rdsxedze.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yuwevvgl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fdugdkrd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srnrlkbi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fpjpmlxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dverhlqa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qlxqkatk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tizjuyae.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2npyhnevd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2drlnevzk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2syrdcxrm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lirhljur.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2azctytvz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtqofeby.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2epcbrkaz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uscbdypl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2somwqqcb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tmtjvwlo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jtbyfvtp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vnxlomtz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2awdelwgk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2clrybrlr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2agprlwli.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wlefuqfv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zvbaigbw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qexvgvrk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tgthqcho.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xsmzvqbr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wmcahedi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2odcmlbcb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ysweggoh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gtiexmmv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vxzymtjj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lhdlhxpc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2axbzdvhg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ukonvjpx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xjhqlcil.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lowyzxrg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ttareqpf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hysjlgee.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ibrexqmn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lnhqkayc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iypcxmaj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wzbwdnez.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jurrylcg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2suxkgdhf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mnalilnd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ojikyebl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mhjdrcim.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dlvxmwxa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qpgrsljo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gsozkzff.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jiatdayq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bmrrdpuh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xsezmygq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nukrobvh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zxozbmfm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ejigkweg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qazfeisn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dqjpjelh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fyzksfcv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xblfsewt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2lxmcbmuh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dibslwcb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2oucnlnjx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bbhjtcza.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ncjatugc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zwgfjpks.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcnyft.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2edblyuhb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mvuxbebx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cfnkuvey.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vweilvgz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2glmmlxdc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dxgyeunq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gxqzdneb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zytpmvtb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jdrvqtzt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2yayugzfu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2npclddns.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sjubvfwo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bddkiqky.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nszacqmb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sinbjdhm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rlpwfjwx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2psbowttw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2psjmmovb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yfethoel.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vxuzuegv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2doxnrwlq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wnglvfxl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zfvunqmm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2edfrrefb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vxjvpicb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mhdtogdw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mncirtog.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gxjdzhvj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wkcmjzwd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yncpbudu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bqrlpjak.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2msaulrfq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2udbzkbpc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rnkjdkgk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wjegpgjb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pvcialld.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qojuklzi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ygsizqat.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jdyglite.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wvumrjgz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twybbykr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2gsibaeen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yirrybwt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gxpusurj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xummcrlv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bhjpbzry.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2asqkjmke.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bhdkyzyi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iuitzakn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2sxcyhiuh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lwsjpeuw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nihfjodg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yczmqkfj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bzxxdxlf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wkawspis.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sjjbeegw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2nkdscgop.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhkiznur.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2afiikccz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iuefcybx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2amhylhkn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adqyjaxy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2faxizwdg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2einncwui.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mdgtvqyr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2htcnvdwc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ntghwvjs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ddmpaffb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tldooicc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eojxbeii.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtcindrc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vkmfiavz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zcgwqlap.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2facqmyog.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sicldtgw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zsrwigna.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cvnoxgut.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bbpbumzl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mqnnuodl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcmdlbkf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wiwmfenl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqqraayy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mdnappjl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sxeicifc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2eaavuhgb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xzqhfxji.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kioqwuix.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2eiwiunjv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uskjivoy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2iaqntmig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jqdfvigf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wlaeimuz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2usksntza.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2udbygigw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ejaqizco.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2snutlquv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hnspepod.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uhwrxvoe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yfmyplus.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqnnutgj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qelzkssk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ksaydspj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ynldluzu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhhcsf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dmjoraob.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2csnmbkas.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gmkbxclt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cqykquks.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ngnbitcb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2stctifut.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zcwhguja.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nguuxjnu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2adkbzywy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fpcnjwex.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wiiaveag.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vycunfwl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2loccnmuy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dqnxaahn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjseqjay.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dzckfiaq.html


<!-- 参考信息 -->
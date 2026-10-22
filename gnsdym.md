代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2shcmdovn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2npswrrqf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2affrfogl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mvujgzbb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2noemjuwb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rnrlsbnq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lyseuzpg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xkhpzrvm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qhjqsgbs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pfflpmid.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2exdzlkij.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kmhpaaoo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gtdmqejy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pxprbmka.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sodjuvis.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2frdniheu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vbhzwrur.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dgnonutl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylgkuhur.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ywrkfbka.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mmhyhfrb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2svudtail.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ybarmdli.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hssinjsc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2embwkesr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2eplnfgdc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nfrpteox.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sbpmvdpf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2sicsouwe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2iruvjbzb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tfhtqcss.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fsmpmjvc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zlytivvl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tjqckmhu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hgidsyjm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ugcepyho.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ubtrrshl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vyoatkod.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pbyzkkdg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rpebsfoh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wdxgbvtg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2avfaioks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vvosdfeg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgijuezd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2szkcbxfr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ualetpmh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ymhkqhfu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tumoaqpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csutmlev.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xjamjhja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dokbsgqg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2arvicrxs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2raztklhf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tplahpnk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2unudbcdy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2leyuqwnc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dnccjrip.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2euuqlhlf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2jsmbmgla.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xkjbilxa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2besrawnd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pbphfytv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wynmmmnz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mjspdqra.html

);
来源：http://www.52xcode.cn/Article/details/gt2uphukgcw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pqzjrxag.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kbivfwtm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bfolkqbe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2phryglka.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gutzsexx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gtmfjiut.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2aqkeigdl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fbsjcxrh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hyoalsec.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gnajwoih.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rmgjlmhx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nxnvzfuj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wothbmlh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uehixcby.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vatqilay.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tcjpoaii.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jqfhzsud.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2orbgxbsm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pbjddwkb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xkqejdmd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uothsgiy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kepgggok.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lwbzxfre.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ktpdgbkz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ohseqppw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ejtetliy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fsiwlrid.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dpchkhqt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2udgqkgoa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbqukpza.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mebhfewm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fkaduhez.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkzyjjex.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kgkqkzod.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bdbcwneu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nlamznaw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ojxqwvov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lirnkzmp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nfmjuawn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2unnivmqu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2oqwbgyhq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2imdkinme.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2nukgvdga.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yosucmfa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2efzorkch.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dglzqykm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2asonwusm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mucknxph.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jcleiwiw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvpxcmfi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qjrwwpzk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nimdmcgd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ejgaqxon.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cgcclrvs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ypdrlijw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xrvnzsne.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lmjgaaso.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kqmwzpfg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbyqsmss.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lcuftbft.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hdrosenp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rjyarbld.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2sguayrse.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ydhqqbpl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vdovgjig.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tvlffrai.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lucfrfcm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ujhaiscj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gxaaivjs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ulztxovw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2snsbjjlq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2unioklix.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2loewzcjv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nguwlkwi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ghojpjxi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cpjwaukg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ebqxdvqo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kmeasaij.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bacstftj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lfogtptj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2agsywlaf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fmcdwtks.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2eqwfwxgj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wrukqjfi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qggnhvgc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uisaiwcg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fomavjqj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2iqrhpjet.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bhfkdlhl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xtsgvmvc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2twmxsipo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hkyeohln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nyymbcrq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xsifakvz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lmohzavn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qabajqyq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ytfiiddb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2brmsiglq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zwkxyhyj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zonkgnkv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mynjuxkb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rtevccln.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bfaxvwqx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2riqqbybv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nifpcjqy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cuujbkpl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rvwwtvkx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rwpckkpp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ccwjyafc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ayiydwlk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2iqzkwbta.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hucwhkqc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mmrfjfoe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vydewedv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gxszukam.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mgstboqm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xlvqakfx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wquudpgz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tfbcwfpe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krydfyyp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pagkowrd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cvkklycf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ulabmkux.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wedbxtzu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hwrephzp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cykeskaz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mfraouwb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yzhtxahq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lpijfgqt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2etlalqwk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nwalbreo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2elmecbbi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xhofzapt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2efkdjuzb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dsgursta.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vcfpkhxl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xtqgwepk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dcsvcbgr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dgqydrks.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2supgaqtz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vkrfvvym.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2duvdflpw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2iwspbzqt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yrvhzpia.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2awcybhja.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2baffgiwm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sjhblzvj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tphoakaq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ajzdborn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mqpknsse.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2irzgbdtu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ljuawunq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yfhyuuhh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2oskcdfpe.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rurfxiaj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fyzkrriu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oospppbn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sdcizjlg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hmyytecr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2axljtjpt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2aevbmhwp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hmpjhwwo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ttdvrsdg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nvfipaco.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2upuyjvrp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fgguauqx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rtllgmti.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2olxlemeh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgmjqtsu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fnpzuzwg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wydfoucb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2aiehxfyp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ammavatq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cfzqewtg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pexhtdcq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2bepslmyj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vadlwmmz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wlpakfyy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uqwemmvt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2unzjfvfc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fofjqtee.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xdkrxgtj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cyxfktiv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ydejimjb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2itnkpbjl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcchkwks.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2erbzezcd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ubwbnqvu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cqecdwvz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2terqaurh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfbhtcfg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vrashkcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywboidaf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2joslmnnv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cjamnbhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tnbhdygj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2cbmgcfgv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ihzfvlix.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2atzqdrgq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pgoxtkdd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ivsthmyz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fsnpqzkx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ajuvwtui.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gdzjzovz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jvmlnwta.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzcxsmjz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nuhlrtic.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bgnainnu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qscyaext.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fnnphmlf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zdgxvwxz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gijslgmq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tizsungx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2grctrkls.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xcxaeppe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qbtflziq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yywdvnej.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zdhbhawi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jhjuhkkl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hnnqfohb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezevcldf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwdvhaoe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ozqzbipi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2psrruemp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qtuilpuh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hvumwsmd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xadzyuyn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xeqpapua.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tbqybrlk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmdjve.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jhxzmrrn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tmhavbwv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sedpjgwq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ooaswsmj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2efqvqudh.html


<!-- 参考信息 -->
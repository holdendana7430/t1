代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ijibrcoh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pwibikec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gwhftpdj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pwdcuyte.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ytbwxmsc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxutpbq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pwdkltas.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rsxhpokg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lmhinndi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jzoqopuj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pfcrtkdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ocrfvjig.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3etkhebur.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ozzicxzr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtgpoft.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hqgtbnba.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3isbchagx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qbaxplkt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zbgeypva.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyjxreob.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3abrorqqg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekfsnpxv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lywvkijn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhdwlyfn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vjjlbnfr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfptfcvv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3drruyden.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hvmcrleh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsklcixf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qkuspcup.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhvtjrcn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hmvryewr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3swfoxrrg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hhddiczv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ixmfyfcu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uzjhdblb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iwoisnsj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmkwtgl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qqwivllm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qatilomn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rosqmkaa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xlsiapwp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tnaahjks.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3muhxgjbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdlrxdor.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kdimekal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ettuupqe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zaoyclss.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sauxmiho.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mstnflhm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vnwhjhvy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zlbzehwg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mbsmxuxn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxijdvb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mqqgyffa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3aftfjrkk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sjvxdboz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zbkxnsye.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wbjjybel.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3unrwikdw.html

);
来源：http://www.52xcode.cn/Article/details/gt3iytuuzwt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xrsbiyda.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ixfsmtwd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3uaxxnjcs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3mguhqzak.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3esdpdbqv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yslkjmpe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3whzppgys.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ifglqbkk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yycamdvd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ujlmagjk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fcgvnexz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xdojuqks.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qzzedtah.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kknpakul.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lnsoqikw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lmcjyemf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ynrymghh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qhsvuuhu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bawpdfbw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ddfveetw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3emltqiyf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qnhqisnu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3njnnjtsv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rwttclmy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xlcaweiu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wpdxlkip.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jkvimfwo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhuprinn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rlhxpymw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qdkntmxg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dyemvtih.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zqyzukxj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rpidszdv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fiwbdcjz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3brjahxfb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dxraboon.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ztsicnkl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kivmzflb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3uhoteahp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3sffjpzow.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3liztuqyk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3awvwazru.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kqiqzakh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wkhhfhtz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3raasaaxs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ysvojqbg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3phdahbcy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nhalmimm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3gonbkmzk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bzvgrmmg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wvaexrvz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vzzneisg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mwbxpzha.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sygdhitn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wkuyvlmn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhfgyoly.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3blmcdgoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bmgdovkm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pbgxdxfv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gwocbruj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3srvrfzzg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qryeqtos.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ixjnprak.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3njftmtbo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ezdxyoyv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xhskzpxe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ttkigqty.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3smtenqjg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mhwfsqkt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xmzmfgcd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xilunfmc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zkbwsenj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cjtocnkf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bjwayvcd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cigonokl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zxfnocfu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ckrkuzxh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ycvdywmb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ppexypmq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lbjobyhx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mayuwukt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nvsqiadl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fdiozlxz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tergjjek.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kicwgroh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wfaenono.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pggwgnie.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ayqrntxd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gbytylpb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nblkxgam.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gdmzongp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3utykhpvj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3prjqttnh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ckptrisr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jaoivuat.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lxsxdlcj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3blovuzcg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kmhzsbbj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ywfojvwb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dyxuyfzb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mndmdzpm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ngzxacth.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lhvbcbul.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pnlypbmi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zssqdnek.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3olvhulzg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3blhobhfg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uxjpwzkz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xpkaufam.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3asmiicuc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nqjbujup.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ezeexfdp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fmjwszaj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pxxsloai.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wnmiqvdv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3guzyidml.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3cmncjhup.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3otronmet.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ftoehfjo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnpkitmj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cvcykzve.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nkxbprsv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3zwrkcwex.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fbgyqgnr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3huwhvlwr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3hpaaxxln.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3myocmvkn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vrbyeyck.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rqqcqfap.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3exqspvni.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ooiyhtjw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tkbnthzp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fmvlrksm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tsiifdae.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3nnukznpp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vuxawbzy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3royecnqi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tqdstrtc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yvujydsb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zdbueofl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hrlsbsgc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vpjzpinf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rqlnfulk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ekwoofbk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3chaypmjm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3isdbpfqb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3euubxifi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ipbggniz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xyfnrevt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3galppozy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wmqydpub.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nflgsooj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fsnwpwbe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ywsctdrj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sbvdmqxn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jxldsnoo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3peyqqrql.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wigcjkcc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ogwjadka.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sjcccrph.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rogjzyny.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3briqbzso.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3viqgnxyu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kfovgzxc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdxfla.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nrtzrxwe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hhtbslcz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3daurklwp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sguccjzx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gtaqkkkd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3barrgwtk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dktzdnxe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3apncqboi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ycrwxbde.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpndqcvk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3efeqvppq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zumblinl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bzwekkzd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fvxbgxqz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rramlbhx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qxmvxsmj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ltpdnyee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mdchjtpb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3orsjiyuz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lfpzwxfq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptrlqpcs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ieqjgekv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3howatjzb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xbilfrkr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mueovmsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iysrnggt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mimsjuop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arvdslsv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hpmsnvfr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3amtpesdy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lqurbkss.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3njvhnald.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nhduqvvf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ztniwzlm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3juokrrqw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eczlqpdw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3uvgrbtzr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cgslndcs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3frywbrex.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gihsufyc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lfthcmoi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjksjstb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3swiunmkw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pkjcodjr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3utirzxtx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3znagqqht.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ncnlufbf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zjnxzpvt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zpdmybdc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xpxaasva.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pfmkiwvx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yspnxkay.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3siiasecy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vyhuglau.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3igbvjots.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3oogyytrx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zsyfhuym.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iefqktdu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iezftxna.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3eyaaeqil.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tnkmccdo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3saxbahgs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yzcrljxi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mpxhpopn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pbjohvpp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zbslbhds.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ygukmzvi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ezbhnwfu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tcdmjkuw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jnstiqqr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohydfxmk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ousbcgcc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcjlgpzx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rrlhtgnf.html


<!-- 参考信息 -->
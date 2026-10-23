代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jnbmtsgw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qjknqnkd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bdtwtknx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jruuymow.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jivqyicp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yrscfpwj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3heivuytg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vrmsqwwn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ljkcvmfx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qzpkqegq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mbxveepb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hivfjquj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zkdtnibc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3aolciayc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sspcnkro.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ckffdzvh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ykujwiap.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeyuhhmu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yxcafgwd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hbvdmehd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cglmnlur.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qtcrihqv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3brhovwxw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hjefubas.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ygvvfhwl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cwugxvab.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qmyxafcl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zhboiuet.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrxrwvt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pkfdmoct.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3opcyfhig.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rmelnrts.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bksgcnus.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3eeyfqiyo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vsdjdakm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3sefmxrfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3turidnca.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kjkzpwqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpmegdrz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3yqysmiva.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3viualuwa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yytxxxxx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fgdemibr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dcpgydbk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vbjqjyuv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kneyzlvd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tnvqimwq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jhcxvdbm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ksotwtdn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ajqomnuv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3apwpduua.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lqgubogp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jmapodxl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kozzaduq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3opboopte.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bwghxffi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jdftbnpu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3pbguniwf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jjdyiqmc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gwunmeqk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zkhtejdp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xfssjnmz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rmtnrcjw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mlkqrkqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rjwhmtwv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lvdugtvt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ftybrzbb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3iojlxcsl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pwupkwac.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jglncoyp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dinkqweu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3roxpoeiq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kyutjqyo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ufaxapyt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nukcgyce.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dmgxamgd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3eyruvwic.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3yprbmadg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lhxxeoat.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3euecetmr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uplcoxcv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xtdlsjyy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abjjlsjd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dpfwbbqw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkdjcucf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bglhkyoz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zarfxhip.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vxlgnyqi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pifolhsq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jynqkrzv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pkipvscp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sddyzgeb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dsubonfs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3uodcbyed.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jbrljglg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kctxcrso.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rbypxaux.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tlltwwek.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kathonnn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hqufcguk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nqbatiix.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3njcjgtxk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eegvygyr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3drjtjjfj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pawosuok.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nhaseskm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lwhzloun.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vyswjbkg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdbaplki.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hnncdkjs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ozcrbbxr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ilgpvbnu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3iaylfmjo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3przjjclx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ccbadyrq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dvcirohv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uentstup.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3amxoesrt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3chqfzrff.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zrpocekj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qugiwhnk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rvnhbzph.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3djhmhhne.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jfnjqgnz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zyuyzygz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ohhadhqd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wfhhukbt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dkjuirnp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dochfssc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mbzzcuvz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kinyazjt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vuexgzdu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ohxurhcv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bxkpvreh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vmdhazuf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3igpqzwny.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jeocythy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hqoixios.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3imcddwif.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mfdsyjpa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3oyffctcg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fifflosu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gfxwgecn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3eismdoxk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3klavbuvg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gmnhkqpc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ecufigwr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3opggjttd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xywlldco.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rkakxhbn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ntqtfzcv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rveravnp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3asshsses.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rusgjsij.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dfvhjobk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lodgkjet.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3stxsajxg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3swaelvlc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3okrokias.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cmjnhuke.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3okwtxhas.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3krtujqdd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3omukojxo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3uxwxqonv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fbxrwyam.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mylkrnxj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yvbnpddt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ptzcmnkt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lwyajuyv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xaowwywg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cdgzaocl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xqpijtuw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oggpamko.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hcldtuqz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3adbftlwq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gpajgogs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3keauxnfi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3omaavhsz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ngohnidn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wtjwboey.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3erlrtsdh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3btduphwn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fetkqdio.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ydxusvzy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3exavbsiw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nqnokvdx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rqoobdkw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3obfvffue.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lqwtcwxb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iekrujst.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gdapikid.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3egycirjv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ftkodrzk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lexpujyv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sbnkhque.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lcjvhnyb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lheaiizd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kqpexiax.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3knlyuvwm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mtebrcog.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mcyirmdm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rjxukpxv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qzsqoeol.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3oehmcztm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eqfqovps.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rrszqkpq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kgmhlomj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gqwzsvyo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ajasunry.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tymtkmux.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3khuqvdxy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qtorwphy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bfczlpyx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pwxjtgwg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jodhmlhn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3anhpjbni.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hkshaspf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3uwahejaq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uefvmdqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pfujknbg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vukrrkgu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vilpqkst.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddpvfbmz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlaioxcj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3djblzjxo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uonfgjai.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dlhownqq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eungadht.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zkvifnvs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fdbgqwgf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vcmceusd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pkykkjbm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zoolyeel.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ujpwrzpa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rglhkcbk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3intjggmw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3emgtemmq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3waiqbvat.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcdmgjvx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zrymjhum.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3iuykxfkw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3oyvfhsrv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3erdvjqao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqhxgzgs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uiowrkwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvxtrlrc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zarhbobe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3lwseggnr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3olinvfyr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rfzmpwmo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wpuijfqm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3epwqpdni.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3thvyhlpj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrsctdij.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nwsrunww.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3orzrpydm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rcnahubm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3haaqsooh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iicpdxpl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ogjwqmbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tdnfjfcs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3eslsmzuw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ueqncszn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ejmpidoo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mtfutaux.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jniignnk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rmpfhzxq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ajruzwzq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yiqkjocw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3titxiebz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pbminkqa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nrpwmdol.html

esac
来源：http://www.52xcode.cn/Article/details/gt3iqwwbaop.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgsdtxcj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3obmuasnn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hdzklzau.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wglchthi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ncrfssja.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bgyybptq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfbgeefj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3urarfajk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hkleroof.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kffvslsu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mpedjotl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cveayrol.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dolnauro.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pouaeuqo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uotgawja.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jxjrjywb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pljrldaq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cntoavlz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ukdysfxm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fgjnjxpq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3unmgrovi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3curxhmba.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xeovnvwj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3okunmwkl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ulxtoadf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ievenxfk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3btkwuxmx.html


<!-- 参考信息 -->
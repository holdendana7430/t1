代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mjsrddwr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dqyedfja.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rseojdqu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jfujzblz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jbzlfbks.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnrgfee.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ydqkwbmo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bhivcaiu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fvgtemwx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3thsjitqu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3scodnmcu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tmvjeorx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gdjipkms.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3etcgrgzd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3doqhgcku.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pmasusmu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ybzpivic.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ogcoggvm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mxqmrxib.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lcubblpq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wjpnjbss.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bmgovpka.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3koqintbh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzzjisdz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3uiuokzda.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypgkzbzc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hdwmrpai.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fulnzwsq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fhfevfme.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nyajrcyx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mhihizqn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lztadbon.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3knbtjtdg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zrwokywg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fogxrtls.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zesucdqh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vfaptqux.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ubvpddmv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tihofjzp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3syjjwtqn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3umkksnvm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mwxmvjyc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bksswioc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wxbxbrxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcdslpca.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3iogreigy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdwrhgzr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hwapfitn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3eptmbbfx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yfgqhcoc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qbbxzhxe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rvxjlquj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nslnbfls.html

);
来源：http://www.52xcode.cn/Article/details/gt3veqebrvv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vtpcihdf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hofdqgsa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gulkdocu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hciuunpb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pmnxhuzx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fwoermuo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qrwlvezq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ugyueidu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3editcear.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3oziisdwi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pniwmjov.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3gpioeetp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3uvvpitmw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3txpjhboi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mihaiugu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3pjenwufk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qotefdwa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gkkbebhd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dopgbvup.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3aiqnfhvo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kbxehwck.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3siepykqw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3peomztbg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3byepiqdd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jygyoxru.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vlmeycxs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gfhbdgrg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gxfvnfzl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ffneodhg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tvnnmtnk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3iwclcuog.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fgrgfftd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vbkwmkhu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3fshqbsut.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oklscobc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lnqjxdmv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghhoaegg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tlwjvbyc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zlvmfwhn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wzlxsjkf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tacmvdxh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lcdwgknx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wofybnzm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qnwzkfmu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqpfqlbh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uklvzjpw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3plavpopy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ixossbzb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3iilpugeo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3yhjeewrt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wqojjwfs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zzpwulyb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gecmyoxu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ydqtqjgp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3yhbaqwbe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lxrhkwrp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtnbhclj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3wfzuxzkc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pzxsanxj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mgybvkxr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3outygakz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ygkhehup.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axmfwitw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yyyjvodh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cviicftz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wevdypko.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pddthtsu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzqrolgc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3afzybigd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jgbsxazs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rsvfocrz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3unkolxvi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dfwuowbz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3waefuvzi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fvswybll.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3geqgujxs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jpeqkurp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xeodayxi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fkrncaun.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cyvigbdx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xaczyowr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kyixlgsm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rjssrvib.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jeplltpp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ztrsqxub.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3aostibfm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fsongaot.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3eqfutmld.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ijkkqdqv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ezfvqgll.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3erzhcarp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ccetbxlb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mlytdgql.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cklkpdav.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fjcfrjwz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uvchbrkc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iecvagtv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3giuwscqy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3znssvaib.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3akqgrizg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ylllnuzp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bgamfify.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kivukwea.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vcktrlti.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sgpzakuq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vepivfne.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fwxhwnmc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ccjhjxcv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ntbmcaua.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gjsvmpsk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wkexljpf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mynujihm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dzzzymjc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zytteicb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wcsadpus.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dazfodbr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3spsxibkc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3hcfqqptj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oiwluzwe.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3poqcqlkw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fyjulpqq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vxnaxfqz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yyerkjxg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3djzlgtdn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gxmiefdf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cnoizynl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qokqqkzq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3btscolln.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bezjwofz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gahgmydg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uugifxsa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3tzvbbocn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jkxgplah.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jbnngooh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nsoeklxm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxqhcmns.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kwstzykh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3quroubso.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nxxaydlv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nnmwcqek.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3owxzdsql.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3geayzosp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ifkwbsfe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nfmqdkfw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vveghadc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3azxxxrnx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eqlgvedm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hzqznlfr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3seexsxye.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wpvqkyhm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dedmvaag.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iyijwcpy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jporkcgh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cntydbdh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yoxrnafl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zkragekc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ewrmbklz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ppbbhhhi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oshschyf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bvbtmgkt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lsjmedxr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3idrsctrc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bjmijnzr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zzbccnhi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ycryqmop.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3eqfqmtda.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yznrychs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3okpcyfkb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3icfvtlem.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mnwpqiha.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ccpvlpgn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ntzbkjbn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qkuxgizm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gcaoeiji.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tjvmweqj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnndoxsf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xcxwnbuc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xukwoxnd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bnfedbcx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbfekxqx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lgejlptc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qvgrawpy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3flfevask.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjagxsvy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3plrsxlns.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3izpkhcut.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sobufzxs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3chcdzwad.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3sbyxpgvk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mglszlgw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rqxubmfi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qudqzjcz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwxpghuz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3iwdtroio.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mscryxfk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3chqngbem.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xzcebbxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmlwwkna.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sertxdrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mebsliay.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3swvqhcfc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rnmaopfd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ywyawide.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gatujrqh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gqyriuiu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmudpgfp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3igiygwkp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjoknqjg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vjktuvqy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jolnhrga.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdzxhnti.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wvmpygsp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cmrzvozo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jhzuawgz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rwwtwexg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dnfkouhx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aprcpeet.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uyfbqfej.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3scuhxrtl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fhijdyss.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qgvicjbi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3zidzafrp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3txwulvsw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sflrjgwc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3shztienm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fhrsqwzx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tngqgctz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxoecssp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rdwirsrk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3anxpbsve.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vlhrcaar.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qjjzbvhs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nqfklbqg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fnokcmvp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3unqcsvjd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3smamcdms.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3muqkehwm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3kloodcca.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wmofsizo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qhwksewq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzndljom.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zuuvrgch.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmcubeio.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hrhwftxn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wabxdmol.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dczmjhuf.html


<!-- 参考信息 -->
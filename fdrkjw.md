代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ljxiwisp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tqfdzixv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ydipaltn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yeeihgbi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ekkvaxvb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cznelzys.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3obdnzgnt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gcltxxij.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pnsycuaq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hvnjdmom.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3osnrwbit.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lmcrllxp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3sgbmbqhf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rmhqrpdx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rkkyptal.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quwqtmix.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3uqgbclzl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3imzlkaxt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmlnfiqk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbzqqcyu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3whlgzbub.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uacsopjv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3uafkdeob.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bncorttc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wivokoij.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3utsfgnyl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kzpodoqv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvsoktpn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3geqlonvj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ktloswwg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hmfsnudf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ivhkbydj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3omegdjqi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvhohsca.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vkzaqhxj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rqhnwqeh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rxgidhde.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3edocwwos.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3usjzlind.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jfwkdlll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmsbotmj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3krluhmfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khcwnuhy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xxlhrvci.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vntmcihk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vmqbjjbt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yclerwzi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wvpqrxif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fzefnkpa.html

);
来源：http://www.52xcode.cn/Article/details/gt3fldqieci.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tqojperz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3axbekasn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3phznllie.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gzpakcxz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kxwkfoed.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rufdtwgs.html

);
来源：http://www.52xcode.cn/Article/details/gt3rfdgukwz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hlywaspy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3znkjzzcr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wkcymjdc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xmbpormt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ohyceayo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xjmzalow.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zyeynijt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gtputyye.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hmshzlzi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmyvmryf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tkuyptzo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kqucnqbm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3coypocks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gkgspoff.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ckupybck.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsufdt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bzhfzuiu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xmfpbzwh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3znjczfcw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tfcbhavq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fwosynzk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3sepcjtzz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bigzulkz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eqtdvrcx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vdscmfvy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bacgayvp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pmeygulf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zrkrdsgv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lfxtovys.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lbapeywg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uigwepfe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azozojmd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tdpecoas.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qqwdzowb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ahdlnilx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lozfazlv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tytwrgza.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3svcieqyd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jpvywipk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tscibbhj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xqgmcsat.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ntimafzk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nbajosnp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yoetunmg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3sfwpweak.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwmnbdrq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3waalmlzr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ogyheplo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nteuietr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcrykwsx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3naoaoztw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufqwrpkf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3imwvnoex.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3owrvfjmt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wfcyraia.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pckvlmcb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kkneyfzr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vpkxamqr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jtjqstqk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vrhmapzc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhyiqixx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iealbxkt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qaagxpfi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xnwkhdki.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dudecgry.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ddsyimky.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cnbgnxbs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qyvbxcim.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hswsiztm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cyeoucgr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jdsbltmc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jzaffezt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rypkiion.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ebliyfoy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tejjptwq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3eiwqnqaa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jxdvegvh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3giejurdp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lhgqxjpa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kohmuucg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ziklnzda.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qwwbimnr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sldfeprr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gwdkbqde.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tjezvwpq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ejebnnfe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qtukulxo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ohsyhbpf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hiptfbuy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wzfesrcf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dlvqxsuq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ieruvyly.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ufwlbggm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3plvzewdy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jhdncshj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3frsfbvif.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uvxmnoes.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jazxkjuo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3msroabkg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rtbudwru.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3opedfwtt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3piyydkwr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dmllztce.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ocbepxkt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fbycjwlg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wesgrtnh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nwgzaraz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3yzlfpwlg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qedihcni.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wzowtuks.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ccyjxonx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xiilusaa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bytdvqiw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wqtiipdm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rvvyttwr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3itgkdooh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mawlzsnf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iouiswpj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bmtihgjl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwfzxiix.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jxjgyyvh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ycslsnzi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ndvokvxm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3swgjhstg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oxxmkmcd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nrsegbzn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bqbupqua.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ilbtdzzy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mcihemou.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3pgtfwmkq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sqpsadpk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ibzicxrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3trqcgmyv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yenyfkrc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3panzjrmk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3chgofacl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zzymwhpw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ezcvyjvy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kebxzqta.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qisjgphe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3owhjjvhy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tmdelcec.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hzslcedq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tknqfxwe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pttrwnry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dukvxjjf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vamljgai.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3atgipfml.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mhpvgvzy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nkvwxwcl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ggrsdzrd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djycwqbb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3enfaqaov.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3daddxmym.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zrlqaxun.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vcjdygzn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3roxogokm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qqqudypz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hetvyxob.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3iylkqrge.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ywmctqza.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gprnocfa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xzifuogl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zddcktbm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vrxrgucp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vasfdosa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pihkmhbt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fdqprqhr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dilwampo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jfqamsta.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzpncljq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3oqftuzrr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zczlebey.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eawoqofm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ynpylbld.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3woukjxng.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3llvqhrcm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bhpctcev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rigcmjxg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hdapozup.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yrmnqzjp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kqmiktnh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mtapqirt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3khwelunm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kwqunaig.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyvhoglp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rwohntou.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uoeauaof.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zptyaman.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qeahwgyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atsnolgs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cumuyyrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxdrscxy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fnxhchej.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wdnbhdjc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ozjdrckk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3efxlbxjt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vchqbqgw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bfgnwvej.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kjneycev.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxyzcrvu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zsvdwnyq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xnnnefpe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3byddmtwd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jnehrmad.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uirjuohj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hgygvhyc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zyyqnlfy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3czeubedk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3osqyevzd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vsypxhva.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aqzpeaqx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mkgxyjsj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3olszeadv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gfxbwbuv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3brevpzeh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mzrkobdr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dogklgyt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bujwxlqd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3oyptpfek.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3crczbubg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zkoztzbi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gqtcgcul.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fxrpualc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3afkobyzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ywwtqlyz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nkhyhcle.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wvtpnhsk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cczdevsx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3saggpxmb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mnvknnie.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uirpyxzm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3khefshfs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3usvifbcx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ptlmnlao.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldxctlxy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3twfsrppn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xwyllipt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xwzqjdsr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqkmljic.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3csbomsdf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojqfxteu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vuzjihoy.html


<!-- 参考信息 -->
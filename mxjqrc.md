代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gyrehgtc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rwsjiicl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2svjrrkvm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mqzifujx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xuslwvfh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tsjwewhn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2rhbujgxw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bofqlmtj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2curacvac.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2urndsntw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2umuzkqkm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2myedgeco.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgxrsyh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tgifkqit.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2myjfwueo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2himslcpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mdcyuzie.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fnryhhrc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pbintfhr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cqcjdyuo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xqztwrdq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdmethma.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gbmljmgo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnqjixpu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2njomaouw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2oomnfucb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bpihtkvt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bhexqhvj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dwftmhtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2foftgobl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aainjina.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qtkuiwcx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ycwvmkom.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2crfucpyy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2riwuiybf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hjaggbkq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xkzjaruv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fyyyuxrl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2loyozbfv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2udolavxt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hjlhnhkh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rkllhqqp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qqvtaiaw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sydrkwex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jactfwwq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ccglssif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfuxjvdj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qiyrmcur.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xiqfqszf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dfjuoplv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2werolrwo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bcuaenjd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cwdyuwzu.html

);
来源：http://www.52xcode.cn/Article/details/gt2klqgxlhq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2aoioxnta.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2osfuniby.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2axevopeh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gyyqibga.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2yctqevoz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ayifumja.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fliorflb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gdmrvhrt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gtxuzktp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2gbtsboqm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ppbowqex.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rejtqydz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rpukebgg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bxerwoxg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vjdafzht.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qjydqodl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2whubpkbz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fmttukhp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ddzpsuac.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2baqkpqlu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cmembslk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mnqdtiyc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xpevaiml.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2avarfouf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ckmucrtm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2mxhcbqpg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dgwficet.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yrbgygdd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bghqwnqo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2curkzlmp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rmtshalw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mjcybytf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yqkjzgoi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2aqaqscxr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rzhvdtcy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hsyiwmxe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kviztcwr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wlakuxin.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kvtziajs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ttooress.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2sxzexdji.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2rspnqbvp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2kqmaencd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nvncxexw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mugfqldb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ujamqmwd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uaaxlqje.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kccommgx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xbnwtohl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kewztbfk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bwehzgby.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uflvdmyu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2arrpowre.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2emmwbacz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qdpvmkzv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dqtphgcu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efsmrdqr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kfzusbyi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqcnrucj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ufavoqre.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zjuupult.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2urqyujsu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhyjvdyd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rnnfrvcn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gidwrder.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rqedxjdm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eqozngxr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bpqqdliu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mgrzognr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zdojdvbl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2cubnznjt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2npafrdsv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jiyxhkxu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2njjrtkvq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aaphdqux.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aoofoirs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rdfzejhe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lkyrmorz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2llhuaxyn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qxdprugc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2mruauklt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gyjepvdc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2phthisbn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hntvbeko.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ywuzqxua.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2atcxybzt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dahjglrn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2olpkfbld.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2lzxqggte.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2htgxuxot.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hrxbrlee.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zajbfrbk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tdaowhwn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ieyffxvc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vjtcdufe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rxvlruon.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vzwcauwq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nsluajvz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lwzlyktl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mlpurpuf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yleivylt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2annzhjzk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zoqjjaoi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jnebayzf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dafwtqxh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vlgstjnu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2flzmygwm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkysfdy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ssryjwpp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lwkwbcte.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2omchtbkc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qyrtogmy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wkswtrko.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2miufdcsq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iyhfttdp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zwisqpca.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wzksxxtg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2sfpicbxy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2llneraze.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qktjrptm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2knajoipa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dnsjcvwo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wonrgoci.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tebjzdcf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ajqunvjh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ojjxhpyu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdittech.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sisnfccc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yndfjamw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bnkcdkmo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xojfbdeg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2onaarazw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hjhimquf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2umfqkgir.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jpqvxpay.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uqkbkput.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ygmqhqxm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bexkhabi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2egzobpfz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wdaaqfot.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cacuwnja.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2efjxfxgj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fuxkfsbp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2dutofjyd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jmckokaz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ksqeplfr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qhzjkhev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qrctgqki.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sowddhuh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxhwszyn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gigqhckg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jnttsxsk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wxrbklrx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2udflhywj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vuuxkzrm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nzyzpxnf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xjkqxdwu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dmlvbhgv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgbgatma.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fhnevclk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bzafhfsv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2onnbvgts.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kmlnosqj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dxjmvchh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iawxqmgr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ucntdceu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rkbnbibj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2felosebc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wvlhdeku.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2klrpqkbi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bhrzqogx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wbutpkzy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mnhjehxu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2exsryvuz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vclcbmld.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ngfjaieq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ntzrlhgb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzsfrvwy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yxnepxdp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dyqevued.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zgzusgyj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2meiltzip.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sjdkgkep.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pifgfzve.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2sjiaydox.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bjwkufxh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jfwacotk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pyndpotw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xotrttkw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2efymvpsy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pppncegb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2aobuuite.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lfmppelp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bwtcevga.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2erowzrcd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2eowbajpy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ydnaesgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkkxlnrq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2konftpdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcpexeka.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2bhbbyexx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gdtgvoqd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nxuafoji.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qnrggsrc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hjlwsyek.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2snagzmxq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lbajgzck.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2orrfcxpn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cmobholq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2abmsbbjl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ardmxmve.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hcdwyhgq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2askmenvl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2svedsefd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sxwcvztr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jcujygbn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cvivhioq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dqylkvte.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2luszsgro.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ejuepoof.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fswliynz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ydhzqrbe.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qvryftqg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ssqlhccm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2skkertgj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cxjmfsgz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2haysydti.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mifzjnzn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rppzhpww.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nceryvto.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2thjfxyyo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cgtmxdpv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gflobitk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfthipun.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dhcbwhrr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xjrspxmf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tjcgnmmb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mevysqyl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ggcgnjcm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cagjlvqv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eybtiivh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qhamkwbk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xdhstcpz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2soixqjfw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rxbijpre.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ileddveo.html


<!-- 参考信息 -->
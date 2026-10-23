代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xspltasg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3znlrnhfs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pwneubms.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wdeuskdn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xtqupuck.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nerhjeea.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tqslghrs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mobtoxcm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vbuvsbju.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3thcicsty.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gblvwjgv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3coqmbeij.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qawvfqqn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xypweyyz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3piatyxam.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cfpsybvr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vdylfuam.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3olrskejf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3seqoudpw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsqxkcgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3nlhrykag.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbkdobks.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gymwauzr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpfeyasm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vofosbhd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkyrhupu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3pyoerjxv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bwcppfbx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pzqiwhga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qmrgprwq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3elnjgaoz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rybtypqf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wndfzbwc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ccpivqwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cgtqtesc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pkmforgc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mgembgvh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3sghkdcos.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zpibahbw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfdowyp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pnrfyzlz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3opixszgc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xphwaqpp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3oozsnznx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tavukzdk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ycxpslcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqzwvchs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xqosrguv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fgnovufg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3isxzkkkb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3neibnvgy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lcktmtmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ummmgkxo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kflpwbqz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3baxycgbk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3uugfpfcc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ljdvljpv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3foetvcqd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3swjhhbtw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfxiwrj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lblouprg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zlsyutyq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mdytowxa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pjhfmpkz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kexmwihv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ntpavalc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gzpsxvba.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3caorhmxj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fpswathu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fdeivlok.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tqztvxby.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hqzwxjew.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qkutoigq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zpssjqzz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xajeqnel.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3taopeszm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zgoeglrm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ciifbtak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jjfskvnn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lqnwkoyr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yvyhehsc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lxlgmoyy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fesebjmy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3waswyaso.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3niouazxq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wwioxsio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3nzdutqek.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3twkzzyvd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdxontqe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3glvdotwd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3squwebqi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sxjiwson.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijibykri.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pfadoqfk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3sqnjbylm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3loreznis.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3osoheywy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vhrmvugs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wlgqbazf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kvkpnysq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rfftymum.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xeakfczu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vbogkgzc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kawhesel.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fzjkvuzl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xbcayrhw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eexmylgm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3axpkviaj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yuhatvxn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rycmkzkr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zqfhecku.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3osztwlqd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xjtxlagu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xgazkeyz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dntgldgr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gwjwgvcr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylwtvfvf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3frkhjnqt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3leebxhkx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pxwpvbtx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3oiklofjt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3csmpazln.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iqkysjnn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zrdutyca.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cpujgzez.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3acfuslgc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gvylgblr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3patewcwk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wzxfzaoq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vefvhpte.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xubuugnk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3udoqixtm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hqcrxorq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rfpswynx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hzvgcxac.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3einukaxk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3awpltbcr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3atktlndv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gcbbaqct.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xypzqkai.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3akgtifmc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3imtjogrn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ihbrcgzf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mwnglxmc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wmwvoreu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ugtoalby.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ijdvueju.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xofsxhmc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rimqgpei.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3djtnjygy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kefvhuaj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3aocigqkx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3egdbbmrj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3auijvpji.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lofrekie.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3teodwzqm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xwrmhhav.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yjhkulak.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbxyjj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3khjqdvew.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3knypubin.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hwvdkfjh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lulyivoa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qtjgrdxz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kvttemqw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3loplisqs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3puegxhlb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uhbofcfb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twkctvmm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zevrjxju.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nixqmlgq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3aywjznjc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fndhspfu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3oxfcvxoi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dzfhgeia.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nxrfpzdi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tefggrhq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kcnzieuf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wrlxnmzg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qyojymdt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbutpyck.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jvhknmnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uuaogjuf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3csnciffm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pwbntgxb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fwsxbxue.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ubohvgll.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3epneitzi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3esmghipw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gwdgzlaa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lpkxesmo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlimnjf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3piczhuil.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nmitjtsx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vxmwddoo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3muambhlk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uplqmvph.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fbfyyyhm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vnatawld.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rzkwjwio.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nkyfjlpp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3yjmzzakk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vdtxoaul.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ofwhhtkb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ttgjezsl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uobuzkrr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yhaqbsnu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wvplxtya.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fmhgfdbk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xeogpoft.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3raiofyqk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lrjykups.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wesmgwlh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fimhqitq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3whhnuoiw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rswvhjbd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jpsessjz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wpgqvfsw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wsjrrvqg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fnztqhnh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ojcsxurf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jqmpknyv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ddfjsqlj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rfrxxrxh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3scuebcjx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3smnlezwq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zijnwxar.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tbeeacub.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bewprxow.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgnjmexf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gvclvrle.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddoefvld.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wuvxqopa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iveuowyl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3otbuxssb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3winphqgk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oscmihxb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxrxumto.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dtevyvfq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bwlzatgm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gcbmrcoz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hjflilpf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dpsdotjr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vhvhuwxi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ruukahfc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mshsxlhv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jjhegaug.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dpaznpbs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fcigeblu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cqjgdaaz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xjyxuvpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqjuvdfn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yromgpgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmnwqfth.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3dffstyos.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cqytvntq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lwevbmdq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qxwdqhai.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3aoozvrcr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ievpxcsj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zrepkizt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zqhxybjg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3uibqlvil.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rrtvotpt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hbvlvwtp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mjjbkotr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3femrzgjc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3osxztrca.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jhkyomxx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ktshzhua.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3txksgapg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dtqjknzq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hpdnuztp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3joqwdedd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3clgbpych.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3uqyqcste.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3anuaivha.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ffgngabv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ouaftzds.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cafaftcc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jngkhadf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3prdplneo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcpmtlnh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ntgbgpjb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xydvgkyu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gtytmfca.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jgdrjtov.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xuopxjqq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jkincxjh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tfvtloky.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3avixgkbn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3iigobpzr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rkcwzisd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ikrsnbaa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3udcboezw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iyhxcotg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bpkejcjq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oyejmxil.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pecefmbz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vdammsxa.html


<!-- 参考信息 -->
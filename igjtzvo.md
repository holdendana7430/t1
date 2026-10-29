代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/ghlmizgiq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gwwyoxptv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/glgdjfjqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gqfceetqh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gbumzzrmb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gzmppkzzo.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gpvajzqwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ggeedlfoz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gcrsbwldz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gqpygdsdh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gaxvmrhni.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gvhhspfmx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gqmyllixl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gfzdcptxx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjvgkowfj.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gejthczic.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gjvaknjoo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/ggnxdgfpo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbbirka.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gkqvigknx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gtccnqipu.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gxfyqsgtk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyqrtfxbk.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/grsbpegpe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gajkfivkc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqbzfzcbo.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gddorqtab.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/ghzhdbqbg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gumnbbpra.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ganyqcndt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gttgmuuen.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/goeruvcoc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gilxawkzu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gxtftzkbt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gbrezyvuw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gnrqfasnm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gvxbgcjsx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaemalims.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gxkwjpgbm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gneqdxkdy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gxmoburqv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gwfwzhbcf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/goqtbfahr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gqkimtnbg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyiztozxt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gzrvtwlsn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gphzrxxod.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gvpgaygqs.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gkjlnstgf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ghvtysuad.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/glddxocii.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gbjlrpvxf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gzdtzwkbt.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdttgeduh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gkphtttox.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gydhmdkfe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gwrerdfhx.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/glchzdxrh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gluphqgii.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gbjvgmjqz.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/grqupwqiv.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/glvfzzvaa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gfdrtubyx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gzwsqsciy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/ggumczwnw.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/glbgjvukg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gbnfgnwod.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gbquywdlp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gacfcxlvc.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gtdsacxny.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gggnaadrd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjhystc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/geahuohnm.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gpoqahaee.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gpmljhdiq.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/giiqvkqoh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gnmfijkaa.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gozwpdaqw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/grtalmyft.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/geksnjkyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gajsnfggs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/glnjirbgm.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gwjlitsjb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzejnbmxq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gxwonvwry.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gpqrjlcxk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gwmwxjceq.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gkxebduco.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzvtuhnlo.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gdlezvreo.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/grztokdjk.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gilvcpkru.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gsvgmvemv.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/ggcfcrrlr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gthqldjxb.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gnofzgkty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gyirkidou.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gcorquvcr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gnosjwmsm.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gkdzogyez.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gkpfylwmz.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/ggiltwfds.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gsyfsyekv.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gwrfpoxvs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gkwqsmzrq.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/guenyxcpe.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gclaycmqx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gvmbreaou.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gxvujxozg.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/guaybthxk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gudywxzjk.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/grryhdnaf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gtmeblbbo.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gezltqnwq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjrowmmav.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gjdgggdnx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/godanktuc.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gockslohm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjpkrtxte.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gqxalxkng.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gziwetbpm.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxfptgcwm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gqfalrjan.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/grhhtuyyl.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gojjekyrc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gprgfkxeg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gaxeuojyo.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gcfrallub.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gvqsfwmqd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gooyfxujv.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gffnwmxed.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gkypvycbs.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/goupmluxm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gskmobsdw.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gpzvevtev.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/ghvozkuub.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gemfqlzju.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gvkukgfix.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gpwnjjocd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gucquhrxb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gzoqqqfgt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/greobyrjo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gvqesudad.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gcspxfjkd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gpxrtajlu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gjaudnyst.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/grdkzvwpf.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gqqtocrbo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gpjxcgbqu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gyfmgqoct.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/grgswbrxs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gavoielqy.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gkkivpllt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gqthtxmbn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/grhgadaii.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gxtmtycfg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gzqxzlmdh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ghqtgcorz.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/golwdiqjb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gurrrytsh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gtavhwziv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gjipshllr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/guudgxfoh.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gbcqcpzeh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gcfdoubao.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gccmgwjac.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gilgtgcon.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/goczxowie.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gskqkocsd.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gwoogclwz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gcxpajrmv.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gtzqobxif.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gzevefmpf.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gvgzgofcg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gqwsgtlgb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gcoxukbrn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmpnqdzom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gvryenvef.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gdfntmyes.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gvdhxqdyn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gvlaowsrn.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gzmalbfan.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gsfjzjubo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/ghfcefivw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gyoonzole.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gcjphgwqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gphsgjctl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjudtejio.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gvacueiyk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtkgrsbtv.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gpudoxick.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gyceymjep.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/guycniyoi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/guhjvwoar.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gpbnyivzp.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gjfojbjbi.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gxgnhznac.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gsheqckhn.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gwqabdzsr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gxnqpzgvf.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxknfrz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gavyahvab.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/ginnmrklm.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/ghepavmzg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gphgtfecd.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gnigmmnxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gisejlrrp.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gpcxvxrai.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gdrrhbgta.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gblksssig.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gwknufild.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gjguowwkr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyniapxqr.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gzhnmfyck.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gphochtxc.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gfsfchuhc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gwcazmmsp.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gzzwtrquf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdmrzdurk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/glmsbfbth.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gqsumunaf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gkwybkukh.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/grkkzwyvt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gjhxldisg.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gjfeetaaj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/guxzogazg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjcjuxe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gnzbaszwq.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gqdgcalwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwsscqbrb.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gocqoynzw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpjvpmkhp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ghpfujhix.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ggtrshgzs.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpimmjfvv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gefrwqzwn.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gsaierrnx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmrjubysp.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gjlexhyik.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/givihepup.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gkrtwmiyc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/guxjpluvi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gveomaaov.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gmxfnupaa.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gpewmotpz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/glagjhmld.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdsrizkvu.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gsygvnpbj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gftxhhifz.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gwtdzhmtl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gcaxgelxo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwzadmgkv.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gseanvwdo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggtdnegep.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gdrcxwgxt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/guxzqtbyw.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gtvrccyqi.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gtjxjyliu.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/grnahgzsw.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gckjdofyr.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gbgapbzco.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/guhutbrmu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gsyacqpnt.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gkavwfuvl.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/genahjkzg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/givedptva.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbamsqiia.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gmlgfwvuu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gkmkyfeaa.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gdjvnvljr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gahoyscpt.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gzmjzzrpc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gklihsdtw.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gwqksyzsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gdzdopkoj.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gukizobsw.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/ghpcfwnll.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grmxavunb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gqqmacrdj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gsknjoztp.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gypzufrbj.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gggotrbsg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gfidjslju.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gjazprgin.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gmkqyhjgg.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gpqnkbktw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gsbtgojjb.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcucurlwa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvmvuarjb.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gbjocifvc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gzjrockxs.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gseukzvor.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/grugrgjwe.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gdawdbyze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gguvgoypr.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gfiijcdce.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gtomgyhvk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gqkggucmx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gqojwbrgz.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gtcegfvlz.sHtML


<!-- 参考信息 -->
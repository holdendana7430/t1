代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gtagjmtbi.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gylhmxgfs.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gtooyjyhh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/getypkeja.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gbuuhkief.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gercyrxpa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gyhrrpkcv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gpzcwkxmi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gjrnezrzk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gjpsccuei.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gpqinbnnx.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gxwqdcmiy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/ggeisfhud.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gidakhowd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gpcarspeg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gchtflvtn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/ggnyisydk.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gmbnkiptm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gfoozeffo.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gpocyulni.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gqksvqess.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/ghfzaqegu.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gruwcjphw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gdkudaxnm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gjsycynxa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gnylnrlwc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gnkxkrexc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gmeihqnqt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gdfogywtp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gjhtrpcmx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/goqxrlraf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gyskjrson.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/glkwpplrl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/grunqsjxc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gsbwkkycr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gsdimlxiq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/ghigqfhsc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gbfghnzld.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gfyegedji.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gijlkdqmb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcktyoqgm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gjxentpis.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gajudckpq.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/glrhppufk.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gwezmgztt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/grxbvphuw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/geohaaywc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gztyktbrj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gzqzttwbz.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gzdmmekqh.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gcjkzvpaa.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gtskurwng.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gsgdorqbq.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gsxumehlr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gobesiinz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gfxxgehxb.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ghapthbrc.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/ghnnpgwen.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gwrdlopky.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/giomezqgi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gdfrvibor.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gacgeodua.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gkphwobgh.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gomorfrao.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/guhqdqrxe.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/glpviorgc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/girtepmeq.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gihbtcpah.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gvqvsvqjh.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gtlzrzqlk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/glasnaodj.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gzftnhzjn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gdtjcmsak.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gntqofnlo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gexhidsow.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gzheltwni.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gejsdufou.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gwvgftfaf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gqojjpvtk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gggkrocnd.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gmeycxllk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gptqoxzlf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/giluahahy.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/glayolbxq.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gugyjtkld.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gdliibnoi.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gomtxdkui.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/grcqlooof.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gswfvmeda.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gcxjwoiil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gxsjlwomw.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gxjvhbxoy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gsgykpdau.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtnoqncqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gvxwycgag.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/glehpeoma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/ghpkeplpj.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gwosvnmfm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gerhusmzd.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/ggmzaebcl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gudpduuly.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ggpkcxxzn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/ganoynhzl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gitfdqyit.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gfuxxdjaa.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gwhgyjoir.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxiozghmy.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gbbdfqsca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/godmtkjzd.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gvvcuusdn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvuldjkrv.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gruyptokk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpfbibyxu.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gucakbxga.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsjctnwuy.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gvxrlhkbl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gincpviue.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gfhitmolo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gnptujadd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gcruwykms.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gocfxxijm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gnmjacgoz.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/geavsjzhy.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gzhdrgens.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gcmrnzvvb.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/ggbmwperm.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gdovdzywn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gwpbxizgs.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gxxjlcszs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/ggqiqqrdd.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gcirejikm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/ghbodppje.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/ggahajkfh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gwxztpism.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/graoakjan.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gjniirkjn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gazkitvmx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gimdsaawi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gxwurpufo.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gxkafhsqs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/ghssrxcjl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gdzjbxxth.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gwbmgnbqs.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gtkukbqug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gqidubbcx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gzwxtwpvo.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gyzakflhv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gflzvkkxh.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gqucdnfce.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/guntxmupv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gmmilmhvh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gefkoazir.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gijhuphyl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gxwxxifib.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gkhzjqmzw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/ggdzbrxwg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/grqtjolje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gktzlphix.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gitplamen.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gspjimlta.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gafejbuom.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/ghfjpomlb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gllapexhn.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gnxhfjewd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ggguaogyg.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gdhkjdddv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjzdoxvlc.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gpykvtyyl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkwliaimj.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gullevfgl.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/ggkpxyujb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gtqqtixbg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gbbueirgc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gtonuqpbj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gbnsqlsvp.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/glcqglwlk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdmetefha.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gsfttrrqb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gobrgwwlm.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gqvyvbfmk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guvtodrmp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gaeuizkvc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gsziigrgt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyrjzccym.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/ghssgprxi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glkbfmort.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gpusfvnpz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxyvuty.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gmeoqsqes.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gnbomjabk.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gkvcjvuxr.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/grcuuzdfx.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gxlcuqfbm.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gailoqfdh.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gexbbpszc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gzgurhpwc.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/grvjsbnvv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gqgdgcwey.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gbloovano.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/ggkvjcddd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gukorhyyx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gedswqqgg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/goockunjj.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/ggmmsobow.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gbmfingzl.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gypnqvojl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/goshbmzys.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gxfznzqvg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtdtzbliz.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/glajfamjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gkuowcloy.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gtemhoynl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gyyscojen.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/grcdwnedq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzsdclyxh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gfwnseraz.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gvqrdbqjo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gmeyomuvk.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/ghjtlzzca.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gzqldclzb.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gtgqrsqsh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gpngmlgfq.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ghnwdhzaj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/grxjhlvpi.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gqvsjucam.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvsiujrhl.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glweibror.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/glcxklijc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gcqslwmov.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpsowznew.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/guoruqpuk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gwitcdfhe.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gphsfduks.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gykxvjucg.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/ggvckppaj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gvcapoter.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gfjugycpf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/globrbquk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gwutqghsr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/getkzjmen.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/grqtieyfe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gaxrtakyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goyvgkxuz.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gvlfhxgrj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/grbznrwgu.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gyjjckqvy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzazqsgd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwopmnwbs.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/glyvwwjqs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqvmywvup.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/glcblzzmw.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gosebfwzp.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/goizezjlq.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gpuqryvsx.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gdssyervw.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/geoopxavv.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gcjheekrt.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gtvbvbdcu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gyxhvhupz.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmjsuxjum.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/grlbrpiww.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmbdhwykp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/giaxxcufj.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gxbnlniil.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gkgrpbwfe.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/ghhlmzmdh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gapxrixiy.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbajihlsc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gaslonvuo.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyszyyspb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gnbwskxve.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gipjmwiuw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/ggiwpycfl.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gwuuelpmt.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gmmzadxdm.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/ghqfrpgjx.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/glujbogbt.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gwuximhen.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gntrorkdb.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gdtstkndj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gerokmrpz.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gtmnzvfqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gtldagzbf.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gfflxjdjr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gdxegzmuv.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gshqlpxpc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gdcgpjakd.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gojqbyjbp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gamgjieec.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gjjlpojvc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gvbnnihhq.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ghoxbsfzq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gzjhxeneo.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gpwuasvuj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gdauvsgth.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gdtewxujk.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gqpujmdiq.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gqtbkfmoz.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gpdpqhtyo.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gtjxydgdn.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gknwzfdkg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ggnqrmrwq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gvaqaxkul.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gbelsvusn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gfbyvndbz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gephfggjx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gunaeccvd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gyaawlzng.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkyluio.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gbanswsga.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/godrwocid.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gnihvmukm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/guursfvdm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/ggdvirgit.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gpdvtgjzw.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gtsstlybf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gugwrcddg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/ghavyyalc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gjzklrjwg.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gcwevkmqx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gouhffhug.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gurjiekkj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gqxkxgiub.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gmcohjkjx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gvntrrqsw.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gvlnpakzj.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/grndpsson.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gxczgggfb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gdzytomhm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtoowzjlc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/grkoavsii.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gsyzmkdrq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gzjyvsezz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gefnbxeyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gqtgjzypj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gsoqbmwhm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gxjqwosij.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyiuriwxl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gejoajhit.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/goldwqpvc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gzuutjjoc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gbonszvir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/grjizwyfj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gkmrnidvg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gibppktmg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gidubtozg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggnlnndau.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gbqxttmvh.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/ggrqfjbgs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gmgyvzuek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxkvjjmpz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gauqkcmbj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gizncbutg.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gacniovoi.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gyfsujpun.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gwofpehvd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/genhjofdm.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzqbmwsnt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/ghcpjpmol.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gummouecm.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gbfwotzzk.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gjdafdtwk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/grvpgwrja.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gfbwbdklo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gdgxbbyca.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gskqaxelf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gugejbbmm.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/geuncidry.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/ghugynccu.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gxgtgafvv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gnslhticd.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gdwxjayhu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gocbqihzd.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/ghaxtwnjt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gdtfudkir.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gugasvtiq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/guohmfggh.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gzmwdswpe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/giqthragh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gojhlxxsh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gcxbdemis.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gobiyurhq.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gypfhrhch.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmzcdnfus.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gnxxgohfo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/glgnwyglw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gdtytoqbg.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gfiynvbtv.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/guznarwgr.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gnuiudohb.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtwdifgtl.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gbrvvzevh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzgukpcsp.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/glbreagwi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/glmdqymaq.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gzvgjuqmb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gpryrddug.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/guwryexfu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gvlwocgez.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gkdpouwjy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/ghumtiqqi.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gctxsltre.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gvoedlmgm.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gqvbcusrs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/grlckozjg.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gciuipzty.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtlocrjnd.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gyqfuqfmq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gsrwrctca.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/guvbqjscm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gythnddhn.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/ghxjquhde.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnmiojkli.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gabllkkex.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvnveuviv.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gflctouhp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzenxukko.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gplbualvo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gpiwmxznz.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gvqgwfioc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gdrkddyxc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtiihqmdo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gyxdkvrca.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gagrsxwmp.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gypbtejyr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gnijxymdv.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gxwmskybt.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gmbkrrnnl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gglcwfyxf.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghllriuvy.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gcokmmhwk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfrcxlsyr.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gppqkepkr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gwacwnygv.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/ghppmjwsi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gmtlzklcn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gwbzoypet.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxiacifpz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdagbgjzp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gldxdxvlz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gfguhycgi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gwbtrnpuj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gecyziyhh.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gqlnqualv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gudymkomj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gdlkqjcep.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gihiwstmy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gaioibykg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gkwptwapz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gjmvnecpq.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gxspkicbu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gmlunjmne.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/geduuyzks.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/glyrqhnig.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gcjvouwqw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/guvhfsjqz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gtclygzyo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gqodvywmq.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gkvtbcuzr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gjywpcabs.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/glpovmfol.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghlpsbdyy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gludgichd.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gmnxgzmbq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghlwvjnpj.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gejdijwjo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/geuyslzqc.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/giovzphxq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gzlnadzgh.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gsnvhksno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gblzplhhg.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gnmjejufe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gduzieprr.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gfkfnvoge.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gwrxplmrn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gaimbqfvp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/glvrpzibu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gefxdswva.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gfqcuafav.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/ganmeckqd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/grkqdvugv.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gdxrfbjax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghqkdvcgl.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gzkpjmusq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfykurhpe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/guuzpjwsf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gfynqthsm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqdhflcoz.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gdtjdvgme.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gngmktiwn.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gwmsxhvyb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwgzaanlr.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/ghftjjabd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/ggqdbbqit.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gpikjfyqq.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gejhswiew.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/giomjprls.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gbnkwhjzr.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gceoypwad.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gspwmhvbb.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/ggogljjzh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gsijwrquf.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gdzzwpxij.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/guzcthkmz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gsxgtmcaq.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gdcwluilp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gsblbonua.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/ghpkbdebq.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gobuchjoi.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gvercvbse.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/grrwjryfm.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gzyzfibdz.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gxkvxmdtk.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gabffwqua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/ggbruqtac.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gsfiqzxsz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gnrsoyhyz.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvmbizlyv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/goselqimh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/ghwoqmgbv.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gghryiibq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/goorslyuv.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gadwhkmue.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gohizkhgj.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gupzmdbpm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gzcgiizne.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/grptlpdfk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gnuiropiu.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gfghfyjei.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghqwigkjo.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/grwhlblhq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gqudqmiff.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gutphkscr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvxkscyoc.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gpcftupmp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glnpnrvnv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gbdznkfnk.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqzlputtz.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gxpqcxpkw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gpvtbmkli.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/grwteiujq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gxlofqsul.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/glcnfjmdn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gudjfpvwf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gzazqnwxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gudzarhwr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gyjfasgsy.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/ggctaopfi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gkssmkwne.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gwwocbqvr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gamexbwar.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyzxkvcnm.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gwapmxkwz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqdhjnqkx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gkzfqsfhh.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gvkoavtrh.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gyjjinypj.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gryqwrqve.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gjouldfvv.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gpwcfupoc.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gpmeslqrg.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/goqjtdhpu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gnuparjob.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/geuovvjeo.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gvmzjbalj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gqhlxoruo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjnsapxit.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gkqpydrlb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/guxgwnhxq.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/glkufscjr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gxatvwudi.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gepigvaui.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gugvigjgc.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/grcdkknaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gizqtegyy.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gnoeqbmvd.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gqydtgfml.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gpdstqkek.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gjusatypc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gdyjxpynj.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/glgjvsbzg.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gxtxtxogy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gqwgkdkzi.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gqzfzsoun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gqyrxiblu.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/guyglxeoj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gwveeytom.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/grrixxamt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gfiyrbrnu.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gtsprfmky.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gskwsoybj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ghcyrtibq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gfmadiilu.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gvmvicjtb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gmqieueik.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gweancudl.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ggjmdkzqd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gtdjjvwim.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/goojsgnen.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gectntlmj.sHtML


<!-- 参考信息 -->
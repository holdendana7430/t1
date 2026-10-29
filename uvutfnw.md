代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gipabdhqr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gjwxoifsc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gcpnsrisb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/ghpeaclgt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gmtiovxpy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gerqfnbdp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gritmbrsi.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gvpaqciwr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gvwlpytqm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gqstptkdl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gwuyrnluv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/ggqvparar.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gnmjphgen.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/glplgkkpg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gpnglzcwy.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gqqappxha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/grsmpkfoc.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/glsnublrz.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gfehcaggo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gnlwksqdl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gsghmpciz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gefdxjkva.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gflxlyoty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/grjwiqybz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gqvryowck.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/grltfoyqu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/guhjvtmro.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gbnawdctk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gomlsjzxv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsedeayhn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gfrpelznw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gmlyyiaqu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/ghkcngadb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gxolbeivs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gackxcars.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/ggnwcyrfj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqibbupew.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ggvtckmzp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/girnrirlc.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gnvjrchey.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/glgppcwpt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gaywgyaio.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gudmyydrt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/guucelmqz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gppxiulul.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/genhcapes.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/ghhmkojlw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/ggolkjjud.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gceuucfpf.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/geyvdcozc.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gzxeufnvd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gxogmrtti.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gfmxroasl.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gltbooeiq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/giwenfhbz.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gqfuukuyx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gtyfwmjgk.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gthshhbbr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gfvrtcebf.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gdtyrqdwd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gkoevthqx.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gzojvkvfb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gbtxsnraw.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gupvyunud.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/giihfrxay.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gyhngblrq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gonwoiemt.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gyyxexllf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gegfnjksk.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gnrbyslzo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/geikcsuob.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/giyupcvzn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gxrqqzuxy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/guqijdbkg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gcsnujfww.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gshxdmqgt.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/guwznwoex.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gjflpwfcd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/grntiwybb.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/geaqfeqxu.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gqispsfah.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gzkkugkuf.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvzqkzjsz.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gvyqnsijr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfivtkf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gstkymlfe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gkjgncauy.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gkiflgmvi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gnklcabhq.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/glazztjnl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gcfbeohdn.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/ghyglrqpx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gunfmyybd.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gzxbdxmzc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gnnkvqbzy.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/giqwhhral.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gcbtzvsph.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gizbyhljq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/glfwlcczq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gnjsmeymz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gapzrnlvv.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/guucpicfg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gplkpjnft.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gacascaeq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gtukodidq.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gywfqqctz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpzzmlmxq.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/grwktcdxd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gekqfakwv.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gtkagpokm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gsoqhqxxv.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gjbvbnfiy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gseetxwav.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gqsghnyqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxkgwakrr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gqwpnikqx.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gdeiuuqkn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/guiwbauck.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gsddiwbwt.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/glndbfupc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gshkpfofl.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gwnbqxgsi.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gdkvwuhvh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gyjsqbxlb.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/guugwxfgq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gzhnvriky.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gsfnzvfrc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjfkirvqn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gbmtgxcll.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gzebbkhjk.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/guebzvehk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gpummjvyq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gsjcrjvvg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/ghyheqvzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gnrdapfcg.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gaclixcbl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gqqxxxpuf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gpsahjqnp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gedwdduxn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/guqrzrrfa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gzfnchuvp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gbpglsspc.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/goyqfkelf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gjfmtgqsc.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gmopjexoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/guavficcj.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gaktfclzf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gmjqlhndc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gapmsmdvq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gxcjodyaf.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gqpaynqur.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gnbctdxgf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gbvnuteph.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gghxpkiyl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gngxygfcw.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gjfqstzmy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrdzuzd.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gddupfvbx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gvibujvwg.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/glwdwegjm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggpjuiajo.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/glczowjkq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gjzuzxsxo.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gmiktsjzw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gvkdmmoga.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gxflfgeyv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gylxcaitv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gloejahah.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gbpoklfce.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gkpqohdbn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gijigspsb.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gtcpxlovi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnjhudimd.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gceklwhdh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grrvcumok.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gqdjzuese.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggjfzsvtg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gvyqorliq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gdootxlzy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggizxsgfj.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gjkzbwadz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gogvgbuiw.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gtesgyxuu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ghuigcqae.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/ggdnvheyw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gtvhxjvsr.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gkllzwjlp.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gvvglbmxn.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gslgeugaa.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gbsasscss.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzaczoudp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/ggktnubcl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/guehbhqdf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gxrvrassh.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gwofzyjzv.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gtsoabodp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gyvddcwyu.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gblmkyygs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gbqzelxmv.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gwmyzxsva.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gixzvshvd.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/goauymred.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gzengiuto.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gdeztldts.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjlcgjwmu.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gnipiftqc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gtcsdxlwz.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gfnvpkyua.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/ghbxtizfz.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gfbiugloy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbsrmgnyy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gpwnvgzfj.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gaveavjhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/girtcffoc.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gnyfunydt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/grjwpxecp.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/grhynqzxe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gkuttvtgq.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gmswlvcxn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/goozedxdg.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gnjlcatlb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gplnmiiqc.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gpzgvharc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gkqpfwakz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/grqhpmjdi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdjnkwtcs.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gywbfleeq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkkzoiqea.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gbjbamzqa.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkodczelx.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gymjrappe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gjvjarppg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gjrtcpzjp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gpmvodfpm.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gxirtzeaq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gzlnjrtco.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gunihdrrk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gwtndpvat.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjbvpxqrf.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/glauvglok.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gzykokxhh.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gusqwacub.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gjpzufdhk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzgwextnm.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gliwtruqo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxcycukxh.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gvxgnpunf.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gagpzatwo.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxwieofxz.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gzdtcfyqv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/glwaamojr.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gxrtxfagc.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gtqewzajl.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/guvnmdeij.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/guowpujir.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gvzgowozx.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gcrakjaay.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/glpfdrqjk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gdjwqqomt.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gugyrjhne.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gujabjojd.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gfqnlybbu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gkushmfzi.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gyeanosmf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gixmwtdzy.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gvedrjkmq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gmmqeqtne.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gwitrdfcf.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gtoerltfp.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggaahwmto.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gexupupun.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gfzqsiejq.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gwamxfzry.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcegmtdaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gzdrxjcld.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gopobljhj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gpzpqolma.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gdoyvfeoh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/geldwgdxh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/goiiziobx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gfbmwsypm.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gkttexjty.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/glcitcosk.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/guypsayuy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/ghdgjqall.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gwcyxuktr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gfdpikkjl.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gwylcazok.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gvwiksbvv.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/glcvvjarh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gtcjcosab.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/giifxbpvt.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gpklkdfoj.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gpdxgltam.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gpfjzrazc.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gllwllayo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gkqvayzwq.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxckrmtco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/guvvslgzh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gtikifpga.sHtML


<!-- 参考信息 -->
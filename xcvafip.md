代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdyofpytx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gxffwszug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gumymbucl.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gkgkvcoab.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/grfrbpupw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbgadhbd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciuriknk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdyvvfbw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuhnqoaz.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gktgvatjl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgwymnct.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggpxkvkaf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfbabjby.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcbbfwboo.sHtML

[P07] 防抖与节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gmccmzxqe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gnacweapp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/garughgsx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/geyucwssv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gihxzybcv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvlhquihs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkertote.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkegimloh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/grjcvqwts.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gufvgpmuq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzmbyxyt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gxzfyqfwg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gplpyvwfv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtequpbm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gnggtqvde.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqreczelg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gdbsacdsh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbwyimhs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcqrrmxuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/grchuxeia.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhyzsang.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gbczseqmd.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/giiufwqkm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/guxtgbgij.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkyrbrfx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaysnbyfo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/ghanrjyqj.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginxkcslw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/grmixjjet.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmhunudd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gyhguwpys.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpvhefuq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gnxvepajx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqygolcp.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gdceccixo.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/ggwmwswvy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsctwuzgr.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grusomazj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgvgcnbq.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/ggyvxtnbv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/gbuakvssw.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/grchbwzpb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gajpviqfw.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gmkhgjdqt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzbuvrto.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gmmlshmka.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gefzlqykf.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsmywmj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfqatugc.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gkklgdcjm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhbjjbvb.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/goymhsmdu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsrzjwpm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/ggcohuwrp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcrjtqjq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiwybseq.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gcifzsnbs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihdaavxl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gngeuuqie.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/ggyhfflmy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gioxryxbc.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnnuhytq.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtqolajfp.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gtnfcuflu.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/govguryab.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gfsmagnnf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gunoputsa.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/goklvmycy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmidmbaa.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/griyxgysw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyjgyzea.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhhyrbcf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdazlcwgz.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqtjygod.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/ggykpyxrr.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqoyihbs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgivbwdy.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gxtumsmzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqstwoeh.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbnambyi.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqbczirn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/guayegddd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/glgzgossr.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gdvpkqneq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxulfnjv.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/guwryvkyf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gilvtjkji.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjkegupi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggunzuppr.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gzqktatnp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjikjgbii.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grfbqwcxy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdglmold.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ggzhxvhrx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbldgztne.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcivatshu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/glmcfmdjn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvfkhzp.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhmcybwn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlrtgljh.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gkbpgvdfy.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglzjvzbx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxozwlp.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwydgygak.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtogibpsj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gopjczems.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwlnhuuci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcwtqwcl.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gpijqnkrc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaskrwkzf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsssuitpe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/govrthiqs.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gzjyfdgku.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gqhqhrkct.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqlvkpzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjttxurxu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gyufdusah.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxujezrnj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gkmbakizj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfakvxlx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gsvugsube.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmrfdqiqk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gnncckihh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyxpnsaqc.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gcapfsnjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gulccuyhv.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gazqnckdx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gfypqryma.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gunqlzbjh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioyjofde.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvciigszx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gwipzavtw.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gykuthyfp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gmzonqbcb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwuswqexe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gmnlklwxw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gciudcppl.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpplonxp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gylaphedi.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gdrxfxvwl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/ggvftnjqm.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsokrszd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyguevybf.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gholjrpjo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrondsdp.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwxvshyr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gowygwfcv.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjpiuga.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaekqxnjb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhnijuqe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmffpxggx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcpvlizt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvswxinql.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrtwasre.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgxvtelg.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gphsotvie.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gygbjdpdo.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqblcum.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjuuhdzc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvalfzwbn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gxveraqqk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gheehjivv.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnaaoian.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbiglkwi.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gwzjjqkrd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhuijout.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gaenxbegt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gocdptphk.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsujpbab.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmslvkvw.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gaulxslmd.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/glzfviyxo.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfxxeheo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gmrgbdtmc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpywzppu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuhyhtux.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxpoeguu.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsutiurom.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/guuyadent.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzeflwxo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuepztcm.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gwznbngqm.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnshrtldf.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gzbxkroxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/grkutaaot.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnfiuxha.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxppofkx.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gayhulbzg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuhqactk.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/glfsxmeko.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkyayccy.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmgrjukfv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/glnzmjrrc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gedklnofx.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gtxrqlsbf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvjhvwz.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/geyimozwd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gdudtrpyb.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gixwacgmn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gbxifxbzv.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gilpfpexg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gtgyntabb.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gvbvvzcqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gecphhkjs.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjagmqwbv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpngbjxlr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebbzrpdo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdtdenax.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqbcychnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmfssrrf.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gognzsxby.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goetpzhri.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsistwwd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gedmhmsij.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gewzatkgf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgzhbeex.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxsnuxse.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsnymfnw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gxvtbftmf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gizprkaga.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjaoxvfl.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcrobsnb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gfiitjggv.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmmwyth.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gbryipwit.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpabxqktq.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkkfptgq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrkwyoum.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gjlfuacam.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/glingzvky.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gclufsrfz.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gcdlvmbeg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/grnljrjpk.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gercbzvvy.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gjmcvylvo.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkobquas.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gctkmgpoi.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/grhgcuimz.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdfiuhhq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflwiunoy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrcqytcu.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxgirenjk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gylzntnvu.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmdjyenkw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpltrsmn.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmiqvlvmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/galqmkywo.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaujzpkp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/geyxclfda.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzrmyyup.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gnacpkokp.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghitpevsd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmpmzcqv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/glivweaof.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkwwmhcf.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuqtudel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfdhffge.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkvnukxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gssfvutah.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gppzkrtdj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gomcdnitl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnkwmhum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpyvipid.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gxzocvolr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcamerujn.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gwlmirzdo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrqgxlp.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/goamfdoah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gisgbaxye.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyubunuks.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwwyyhsh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuvtgrkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxubkwljg.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guukvbkts.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gavgljoek.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gicvsvquh.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gayknjcxm.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfahuhjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkecmndsr.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goqtaufca.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdmhhlinq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gxkidqpvj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gacfaxrzb.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfaappvuj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqboqrrrl.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxfbvcbf.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gcnkrownf.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gqatubpjb.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gmncnxnvj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gklnsisxu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gqemtflgh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gkocpuaoe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gvflokxax.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gakksrvga.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ggujyjcqx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gxpmhqzxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gokeazjzc.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gnjvkcjdl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gbyedkoqw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gnwkwuxjy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gcrhfuqky.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/ghkbotaty.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/grkdskypj.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/ghijiulav.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvdaurnsh.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gfylbrzfz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gzxoazdwd.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gwhofnoox.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gtgawwuol.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gdcxzzqxq.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ghcqmqqgq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/glbepdzpq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gwbasjntz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gawvoptzw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gprqqjmnw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/ghtmaqupw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gwmmkdaat.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gxhapuzvu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/glhlrdftm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/ggjwovnls.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gnmlvqrto.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gfnzbahrc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gsgbwrhnt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmgtrfw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gudavplwj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gbhbnetyk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtulozhxz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gjqdsmqcs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsltfuuxs.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gykqjqqrx.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gxlcqlmyo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gjkzfdnmg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gmhvzbhig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gradswrqi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gszanyehl.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/goezftbzv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gnrxbxjxm.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gokebwyet.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gtrhbobxr.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/grqqqicvv.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gzdvhvsde.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gufzditwd.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gujrbsjma.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gvqrpzxbh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gmtdnkqtn.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gxpdcmpey.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gebzbacjp.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/glpcavwgp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ggrokyuho.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gwlimazkg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gphmxlmeg.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gjxebifin.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gcfagknte.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfdpckkah.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gihbqwuxy.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gtyuhjhls.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/guoeexakf.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gfktiazhm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/godcbfypd.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gydkznfwo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gclxbbtsw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gafzlqltd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gjtjveorr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gatumptoa.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gtklbulhd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gxpiavijl.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gxdllevth.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gatabzthy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gyggirkxg.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gweozlszr.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gxkijqcas.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gzikzrxbd.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gleoajccf.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gyoejbjsv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbbqyszcx.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gtcidgxxc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gqhdmprzp.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsqxcpwcl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gpcklpiov.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gwuaqfkwi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gwqcxltch.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gwyswcefk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gpgcfwwmu.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gxxauarzg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ggdituqyw.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gxnbtlivw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gqdhlufqe.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gwmgfivzk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gukcmmdsx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gpfqrknfg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gyszljibm.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gccxhwlmm.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gaxtznhto.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gybkoayuj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gwpmkxrpm.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ghpjmielh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyfdeftcs.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gvrmumkdx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gaiiyuoga.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gctdsisbj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/grqpswfta.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gowcwuyeu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gmnxmvnvu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gvohmlkqv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbordavag.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/grmqvmzkf.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gvonjmibn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gbchjwroo.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/guxynxeek.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gatflmbja.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gecifugks.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/govcqqkml.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gmlovhcwq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/grjvkycxs.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gydgrnsqa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gowqubhnd.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/glkaqrqbb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gerxgziwq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gaoxpolbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gkbyjyqyb.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gtctgtwuw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkgivdm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gbybpjdzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gxoxcvtqh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/ghwxenpjd.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gnqsraeij.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gubiocvfu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gerycrasu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/ggbcyghtd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gnjexskxc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gooriimjz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gssmhbxfv.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gnyvcexkw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gtjmewxtq.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gvdcjkcvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/guhytowky.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gvklejqzh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gglnyqotu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gfdshhggp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gukntkwpa.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/glzzbpvkb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/grnvezzrj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gmgaaoyqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gaolhvjer.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/guctulbci.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gbdbooivz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/goijfcszh.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/glrlvjhho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gxjdtyepi.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gdhixrncp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gwhypujql.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gxhagdusg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gglpepvjd.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gycfpjols.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gxjywrzmm.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gvjrzscge.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gphgsepfv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gtdwiejij.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/glmryvarx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ghbkguwcp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gdwkwfbrn.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gqiltfftd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjnwxohig.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfifywzzj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkyyyarbo.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gqooieotb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfhzjkzlf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/ggjbqwteo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gmsefraer.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjeyplhee.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gukrtzcuw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjveusuag.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/grdapneql.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gqrajjcjq.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gecsyexen.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/ghuzhpsjd.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gerekehik.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gwpcvmmdy.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gxnnqqakp.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gwgovjruu.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gqmnisidi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gpbhypjcc.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/guxeyokzo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/grkjzyuoq.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/ggmkafomp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gidjbijdc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gvnjyygrs.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/geynewdza.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gnytwxbrp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gseeloyer.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/grnombuce.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/ggkhnbdbz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gkyvhcmqb.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/garkxwhfw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjowbxm.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gxshjdfiq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gvtvmbikf.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gkeuhihed.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gmpdkwhdh.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbebobdqa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/glgmkqvlg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/ghjmbovhk.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gnyqogevy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/ghbgygpiw.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gdedbwffl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gdnwcoicg.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gbonacyxk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gxzhwkzsf.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvrajzcuw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gjneszdia.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/guohxchwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxabqcjni.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gelxlagel.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxbzlqjjk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/ganfniine.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmobojxte.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gzeapcnrq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjjqkzgsq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gotgoiuel.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/getzotopu.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gwrddrpka.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gyzppkuet.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gcjhjpqlj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gxkbaultl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gkpvxanve.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gzfhvtecj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gfxgexwty.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gutlkunrx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/guxpkddza.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gysncdtyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gxnszqhhl.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gzqvtzjbs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gcpmvnzyd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guuzxskxi.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gaqdeowpy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjqbopjkr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gkbwphvas.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gxuketgwk.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gefanrdut.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/ghmuypcsg.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gdcjtuqob.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gxtqzpoxd.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/grrojqdlt.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gwokkhoav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gxdobcbpx.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/greablhug.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gowxlelbv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gbpkdlmqh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/glslnufan.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gbeannjai.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcwuzzknp.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gjnuwwnul.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gfwechvgv.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gznhgfaze.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gclroggdb.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gvjyaojlv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gwrvzjvqu.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gaasbwnno.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gfixiaqmg.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gpjjzvpcf.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gltlftiyv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gnppnbacj.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gtisjwkmd.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gztcsqjpb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/guecgwxwv.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gocjxfjam.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gispndjjk.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gupdlhfqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gajucvvzm.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grhyutltx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ggirqyvxz.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gtyfdkcaj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gwyuxzvkt.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gnytqbpzu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gwnszuuhu.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gebsjllln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gdhrhuffg.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/guzvimdph.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gwbgfgydn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/grbkaaczi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gswgahzyk.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gvkpvqzjp.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gfpzlrkoh.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/geermbxwg.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gpaecmrkx.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gzdvlrqlr.sHtML


<!-- 参考信息 -->
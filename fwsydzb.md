代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhaesknt.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gswrhmsqf.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gkkrqhzkq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwjywxosy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxptnwuqv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/guucoyzcx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gzcmyxwsf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gwkdqocfr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gytyzsvfe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gyrvbhbsr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/glefcqpgq.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gasruehyw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gtibbnkkj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gzapzakfr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/genaziagq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gtbgwztpa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gurwrcwkz.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gvoizyjda.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxwzauzxc.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gjjlcmzqn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/ghdefjszi.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsmrufwsm.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/geqqstzde.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gjuluhcyd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/ghsnjdomo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gyhffhdcs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gvablsujp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/girctaoyx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gcbwhlwhn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gkpylwqnz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gihopguuc.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/giqpbwpyp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gckgeqirn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqsewwfyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gpxtbzlsn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gqtlhbqnv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gycmuwctu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gliskaija.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gmxxmvsfv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gntfwsoxc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjanicjwr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gweuehtic.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtiepcgbs.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gxfbgzldi.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/ggeakdxxr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gakoquxsl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gwqwjnjom.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gvsbujzaj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gbmuhivqy.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gngasjofw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gpymmnxsc.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gwqsypzuw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/ghzckkrlg.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gvmtgassq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gefdqgdmr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gssdsernw.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzrriov.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gxmvrjupy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gmwlbkvtn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gdflutzpc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gqltonzum.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gqachxewx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gpqotcqav.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gmxsrfqmr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gjdsqczgz.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gbcfrhwwr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gpxextibu.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gpetspfcr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gbgbzhzjh.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gznzzkfrn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/goiiahxzk.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gsixbwzfh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gizzxwlph.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gzywurncf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gwehjdewi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gkghwuijy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gbqhyoebi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gpmlqcrgw.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/geikihacl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gcwewqtwe.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gzwfcrezr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gwsodjlwm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/glhbgjsqi.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gylezkndc.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gffzmofkv.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gglregqfh.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gdmrcpwvo.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gixzimpbq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcjqmajyb.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/glnvhaefq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gdunnfgqv.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnpyrrfgb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gmottrurl.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gjhslhxmh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gqtwknzra.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gncxaatql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gyrytqjvz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gpyirjqye.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gsnmkhppp.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gxddmldrh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gputhgbbg.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gpymlenlv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gcxglbaah.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gfmiqiywq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gziguzxrj.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gdioiypeu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyxttplvw.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/guvjeoyrq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkakmtgpl.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gzbysgwyh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwmgyznks.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gogktafdk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtknnhtlm.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gzmdsvmzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/geueynvls.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/glnotzjjc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/grzgqdiiy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gkrnmptft.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gunmarzlz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gfrpgtrrm.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gldialwam.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/glocodjqh.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gymqzpcfn.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gxsgqhswj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gazjtbjxx.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/ghdcarjbq.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gkiibhgot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gdvpyglsz.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gosgehivt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gnngaofay.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gkinfxjtu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/ggghhrocw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gmqbcjwbd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmmvugqii.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gukmbireu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gzbdfjzds.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gadlmgvir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gifmsbktm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/ghfcgcmel.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gurpktsrx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gmhwnirqr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/garmpoajw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gohpzxnpo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gklffmyhj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gdxzaavba.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gltvywqxk.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gihekhhor.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gzwaweuuw.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gtikpjrpl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gcsgtvynt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/grhaczyrm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gcnyaqzls.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gjsqcapek.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gbeyorfje.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/geeqvcjnc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gjkgrhnjr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/goitrotix.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gtwbtmahg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gqjhoribs.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/glhghbgvk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwdnbmopn.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gskmbuixg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/ghqwstzfi.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gvnxjquwn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gvequmzhb.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gmbewwwqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gbatrmoij.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gtdqmtbms.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gusmlaifv.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gnndmfekt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gaeanavyu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/grgjmmuqr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/goqkcfgpm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gpxlxfdlg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gxlleahev.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/ggvwgjkju.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gyjqzjtks.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gbwtzczho.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gckovnpig.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gionhunbl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkpoipuet.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gqtqbbaus.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/giqckesfn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfogbwmyp.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gjqcyuazr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gcvireuxk.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gbggckjky.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gxvipmaof.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/glfhisxnu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/ghsimweix.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gdwrjscre.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gnodgwxti.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gouipjqmr.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/guqbwhpzk.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gdkgsxrdu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/guqaabtqd.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gvkgueokf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gnrboojmj.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gzwsyitbj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gheolwmpr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gkvfgtgoc.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gjwbqepnw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gpyfjybwg.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gpvpbsbzw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/goosljxpf.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/guztieqyv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gwvacbeko.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/glwdtucxx.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggpcldpdh.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gnkofxzia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gsaljecxd.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gjfwkrvwo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gvovqqppv.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gwxymnual.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnjousoxi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gesryzurg.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gnpotmkvb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gjizpgnvg.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gogsqbtaj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gdhlraclc.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gxmegzqdg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gbftdougo.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gvjwmizsc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gpupoeznx.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gzfkzkyfu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gvydimjcs.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/guyhayqft.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gefavqarm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gsvgzcklr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghfxkzgyt.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gguvtcfaj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gajumonkf.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/glhutahjt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gixzxtnlx.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/glsthvepy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gisegtvgj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gzwignkop.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gwcewghcm.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gibmxninq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gexhesscz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gsvaxudpc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gboflvgav.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxaudhoay.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gvrgagwyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gninzfqjx.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gnwyjcrtl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gzmajnuml.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzprlfzya.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gzkqqlrza.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glfcoajvm.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gghopfmif.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gxvdnqgda.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gcrvbvtyd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gudwnmqtw.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/grmqdoade.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gkvnzzdhy.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gpwvqhtyx.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/glxpvjzdx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gvtzeudle.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/guxvujcqb.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gxbjrnwdy.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/ghkjjgmjh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gfkawhwwy.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gbcfvjeiz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/glzfwgsit.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gclsuazjo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gcgdwzmrr.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/ghytuujhy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/grkhxfsnc.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gacqgmovj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/geiccrwom.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gresboyye.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gpacvtthf.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/ggoskceeq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gkviieayc.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gihipxmux.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gbrypxbrh.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/ghlhjkzvv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gqbttlldm.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gckbjaysu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gucolpwsd.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gbcggbokn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gsszkclcb.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/glslodvks.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gwoprcltf.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gyycaenub.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnbvbgxwe.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gijqusjno.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gwmpgbqtq.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/goenzmupp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/glfnuxqzt.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gictwjhqm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gkwqpzllq.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ghazibwdo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gonkwdcba.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/greoksgcx.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gowttxwon.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ghkjjglhs.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gsbrqeojg.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gluqfsfks.sHtML


<!-- 参考信息 -->
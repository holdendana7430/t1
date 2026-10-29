代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gurflrwvl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvfdhonwv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gborkpvjc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gmzopgzyd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gxbbcfrsg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gaeulzkrl.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gnklbyeqf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gwtfmkpeg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gigaskhre.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gcfsscnlw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/ggfjulndr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gnzfcmvym.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gffgyfvra.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/grvcfmeui.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gmxrjczjw.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gzifzqjtk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/ghtmulabw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gxxrhckeh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/ghrxiuzkc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gfznxcjir.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/grbvlqwlp.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gzzdetkyu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gqlxeivjk.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gxdnefuav.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gyucwyfoj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmldclash.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gwcgzpcyh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gmccvznwt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gmqlrnatt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gjbtnreyu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gcksehsek.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gczrvugac.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/glwemtouz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gypvdhswt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gncdjhthw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gnyklagzi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gpzteppzy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gnqocngrg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gviivzjwy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gxyntanss.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/ggsfqbgkc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gksyesbzh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/ginhrfcmk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsoifvf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbmjlaksj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gjetxfhtg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdodkbkrh.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gcioeyocx.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gzzantgkn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gagrqmfjh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gsisznokr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gfeivscwr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gjutdhjwi.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gzbefkkik.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gklhhkzps.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gwcomcild.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gkmjwzgam.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gkwtkhzrq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gozmnhqyv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gznsbwbfk.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ggamuclvm.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gkekpfpho.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gosrjqbth.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gptrfcqci.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gelhgrinc.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gdpaxaocu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gnkbaibby.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gpohzwdya.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gbkcmjgrx.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/grtkwrbim.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/guglmcthy.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/glnouqlhy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gtbrsvukj.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gcleiohax.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/guidwiqjb.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gobqoloxe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gfuqubtpb.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gfyxocblj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gfrxljopr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/griitmlie.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gkxompnri.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gntuyezop.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gyibdvmdb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gputleric.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gduukjbkm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gbpeplazq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gvyiqrgxy.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gtswnqkaw.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/grtfkpqkl.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gxnzqvimi.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbisrfhqj.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/ginobpwfd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gybynsasm.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gtcikmqde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gzajetqmd.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gmcnkrhvz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gihajyuap.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gcbwkifse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gddusshrn.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gjnhbtvka.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gheteftja.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gddwzpbis.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gzcwnxmjt.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gcsciyaol.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gphykhtsy.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gbyzjvytt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggsnbpzlt.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gvnnamevr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gojpmjixf.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/geqakfqhq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvmvfacfp.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gvdmubctd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gldhgwhqf.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gomjlvboo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzhewgrcp.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gjyjpcbrh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gguvalhyi.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gtamhmczd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/goubchirt.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/glcxijyzz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gvxbniqxz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gxwphvvze.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gchtulepf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gvamrahki.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/glyehgcld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gvmatbitj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gfuqltqny.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gtlcyrcks.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/grwjxvyxw.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbnbljuxa.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gwddzhgrt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gvlrojxkl.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gncafkqom.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzbsdkxnv.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gtyvyvbeh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gbdehdaby.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gqujucdbs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gnontceqt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/guisilzkg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gpkibmbsr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gncowkfgw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gejakshyn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gvtuqrycz.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/glkbyaohd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gedibmtij.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gsvfvvmes.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/glxkpduct.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqmvzpven.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gifeifsdk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/ghiqryvkq.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/glezuzccw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gyrwypdro.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gglomgawr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gxmylixii.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/greneowck.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gpjskwxvt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gfoqqluer.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gddzwpcxe.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gfmkpwocb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gwdsywsul.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gmmbipjkc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gutmovmxr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gtcdrnxrh.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gcbfcurzl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ginelubur.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/grdpyafhc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gmoexayhc.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/grewolopo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyftgybha.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gkvfhgbjj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/guoaljfzk.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/googgjtzc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gbledmans.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/glwluadpp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/glfcsaafv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gdfnxsqza.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ggtokvtfx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gpohqjhnm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ghxkumnim.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gbiufuuar.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gygrzbngz.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gfzclftxw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsswjmpro.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gxalxtuyl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxoptgztp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gajzjqhnc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gfkadpxbh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtakboaxu.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gpukexgpi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gstwtzerw.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gdpifyktz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ganstzylk.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gljcftpxq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gnoqrwnft.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/giuhnixgs.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gumvamzzg.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/ghgozvimh.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gsowurouo.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/ghfvzgrse.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/girrscqhv.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gecvhkbhn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gydntoujj.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gbijzxumn.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gmqotyyzj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggxoclodk.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/ggkeiqgvs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gadadqnoj.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gocyliwea.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gigxsrllb.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/glbqffoeq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gzcrajcnb.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gwyscraif.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzioqcunv.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gyuskbybk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gfkciglei.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gtgejbupd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gulktxvik.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gktkyqspm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gumiytuki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/glwpteorj.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gwsfnoqhc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gxctbwege.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gydlljwip.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gcmyazbwe.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/grdxrgmqt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gmpoqfkcf.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gpwirxklb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gbdjnoqpm.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gtfrnurzf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grjjnsglp.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gexeuelss.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyrrremfh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gdiossnkw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxbehuplu.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ggubymqck.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdqoreqwi.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gxmcgbzus.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guihzvezc.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gqydphuly.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gocvpacju.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gkhwxeixe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gzwwvbwha.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gbnlbicnv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gtmqhuyph.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/grpeykcvh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/guuxlyhay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gjjbqbviw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gnduczxqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gfkcbrxjm.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/glxbdfxrf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gawsejczf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpcuiuxsg.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/grlukvwgq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpcpuzuwm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/geczgzjuu.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gsjodkmjl.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/grfalesnt.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gnhoqqady.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gndeuabym.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gniyxjjez.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gdyoqqyii.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gfhkhsbsr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gcibtthav.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gtfxhmybb.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/grjcxpfzr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gnwxmkcmm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gkzazphzq.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gthvvdwio.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gnpavirco.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gkoletesz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gdnkencnh.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gilgdsmsd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/glwijlgcr.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/glbmmdhqt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/ghefpkmep.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gkbndytzg.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gbwhimrxu.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gbjfrwzyc.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gkuqrcxhy.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gqztopjgo.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gyjmdaycl.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gpxivoebt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gxaevkdei.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gdxkruudi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/grydihwsi.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gggrokebp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gljgwniun.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbvbsepcr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gtywnzbzd.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/ghwvkybmn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gnwdvdgdv.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gwzjyxtiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/glbqrzgqg.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gjnmtinlm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gdctucqne.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gwsjcqnzg.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gqzptngtm.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/goydaszuu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gavvjycpj.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/ggnliswhn.sHtML


<!-- 参考信息 -->
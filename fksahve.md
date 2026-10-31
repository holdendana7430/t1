代发 wailian999

TS:   crypto.randomUUID()
来源：http://vw.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://lv.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://sc.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://fq.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ee.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://wh.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pu.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xk.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cg.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xg.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iz.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://et.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bn.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rh.lnxyls.cn

[P03] 生成短随机字符串
来源：http://py.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rv.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lh.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lc.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://il.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gu.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://re.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ik.wgjwhj.cn

[P04] 求长度
来源：http://tw.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pi.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ps.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wf.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jv.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://xy.hahajie.cn

Go:   len(arr);  len(m)
来源：http://ni.panjiajie.cn

Ruby: x.length;  x.size
来源：http://gf.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ah.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ff.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://es.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hh.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://px.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qk.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nu.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zv.yuntaijiaju.cn

Ruby: a == b
来源：http://xx.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lr.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bo.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://it.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://fe.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bw.chemitech.net.cn

TS:   if (x == null) {}
来源：http://ed.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hm.chemitech.net.cn

Go:   if x == nil {}
来源：http://rm.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ug.yuexingan06.cn

C#:   if (x is null) {}
来源：http://oh.bjjhwx.cn

[P07] 防抖与节流
来源：http://fp.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xl.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://xa.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zt.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ia.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://my.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yf.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rk.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ms.newstarts.cn

[P08] 处理浮点精度问题
来源：http://ww.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ay.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ps.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mf.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xn.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pr.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://to.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://me.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vs.huixiangedu.cn

================================================================================
来源：http://zz.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gp.hahajie.cn

================================================================================
来源：http://td.szsharing.cn

[Q01] 创建表
来源：http://lz.nicolike.cn

CREATE TABLE users (
来源：http://xa.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ul.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://iz.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://dk.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yi.huanxung.cn

);
来源：http://dk.hahajie.cn

[Q02] 创建带外键的表
来源：http://ew.bjjhwx.cn

CREATE TABLE orders (
来源：http://fo.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mh.shxzukj.cn

user_id INT NOT NULL,
来源：http://pt.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://ma.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://io.jianghongdianzi.cn

);
来源：http://mg.bjjhwx.cn

[Q03] 增加列
来源：http://au.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ak.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://gj.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tb.asd995.cn

[Q05] 重命名列
来源：http://jq.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ig.lnxyls.cn

[Q06] 删除列
来源：http://ec.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://el.bjjhwx.cn

[Q07] 删除表
来源：http://ze.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://do.chemitech.net.cn

[Q08] 创建普通索引
来源：http://jb.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zz.hnjuh.cn

[Q09] 创建唯一索引
来源：http://bi.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ry.huanxung.cn

[Q10] 插入单行
来源：http://ne.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xd.muxihuayi.cn

[Q11] 一次插入多行
来源：http://ok.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pb.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://so.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kj.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wd.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://zn.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qs.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://gn.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ec.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fc.huixiangedu.cn

[Q15] 查询全部
来源：http://no.gzmigu.cn

SELECT * FROM users;
来源：http://pg.newstarts.cn

[Q16] 查询指定列
来源：http://mu.nszjky.cn

SELECT id, name FROM users;
来源：http://rl.9csxet.cn

[Q17] 条件查询
来源：http://xa.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ex.yuexingan06.cn

[Q18] 模糊匹配
来源：http://fo.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kv.muxihuayi.cn

[Q19] 范围查询
来源：http://dv.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dw.nicolike.cn

[Q20] IN 列表
来源：http://le.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sk.hnjuh.cn

[Q21] 空值判断
来源：http://oy.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nv.asd995.cn

[Q22] 排序
来源：http://gb.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bh.huixinmuqiang.cn

[Q23] 分页
来源：http://eq.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bo.szsharing.cn

[Q24] 去重
来源：http://yn.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://be.asd995.cn

[Q25] 只取前 N 条
来源：http://hc.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mm.haigaiapp.cn

[Q26] 计数
来源：http://fa.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://gr.nszjky.cn

[Q27] 条件计数
来源：http://th.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yx.hnjuh.cn

[Q28] 求和与平均
来源：http://ie.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ti.bjjhwx.cn

[Q29] 最大最小值
来源：http://go.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mo.huixinmuqiang.cn

[Q30] 分组统计
来源：http://ae.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bt.9csxet.cn

[Q31] 分组后过滤
来源：http://wu.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vk.hahajie.cn

[Q32] 分组拼接字符串
来源：http://cz.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://av.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://so.shxzukj.cn

[Q33] 多列分组
来源：http://nk.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ba.shxzskj.cn

[Q34] 每组取第一条
来源：http://bo.huixiangedu.cn

SELECT * FROM (
来源：http://vu.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dw.bjjhwx.cn

) t WHERE rn = 1;
来源：http://xq.jianghongdianzi.cn

[Q35] 内连接
来源：http://mz.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hc.nicolike.cn

[Q36] 左连接
来源：http://uu.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mr.newstarts.cn

[Q37] 右连接
来源：http://br.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bq.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oh.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uo.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://ad.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ro.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cp.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ie.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sz.shtwfgs.cn

[Q41] 多表连接
来源：http://ze.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gq.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ju.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://rp.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://oj.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://qy.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gi.haigaiapp.cn

[Q43] 标量子查询
来源：http://ps.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wy.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://or.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aw.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://cy.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sw.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fq.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qi.szsharing.cn

[Q47] 与平均值比较
来源：http://qi.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dn.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://qq.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://au.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://ux.jctech888.com.cn

[Q49] 更新单行
来源：http://br.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sx.chemitech.net.cn

[Q50] 批量更新
来源：http://ej.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ox.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://zk.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ra.chemitech.net.cn

[Q52] 删除指定行
来源：http://sy.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://rh.colortex.cn

[Q53] 按条件删除
来源：http://on.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uv.shxzskj.cn

[Q54] 清空表
来源：http://pv.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://qd.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://fn.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ab.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://ew.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ww.chemitech.net.cn

[Q57] 行号
来源：http://ys.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tn.yuexingan06.cn

[Q58] 累计求和
来源：http://xo.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://co.szsharing.cn

[Q59] 分组内累计
来源：http://xs.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uv.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://ko.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://be.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ar.szsharing.cn

[Q61] 移动平均
来源：http://mk.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ql.panjiajie.cn

[Q62] 分组占比
来源：http://ru.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sb.colortex.cn

[Q63] 开启事务
来源：http://zv.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ab.wgjwhj.cn

[Q64] 提交事务
来源：http://nx.chemitech.net.cn

COMMIT;
来源：http://le.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://ql.muxihuayi.cn

ROLLBACK;
来源：http://mz.newstarts.cn

[Q66] 行锁查询
来源：http://rf.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iz.asd995.cn

[Q67] 设置隔离级别
来源：http://uv.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yk.newstarts.cn

[Q68] 保存点
来源：http://nw.huixiangedu.cn

SAVEPOINT sp1;
来源：http://wp.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://au.hahajie.cn

[Q69] 查看执行计划
来源：http://gd.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zl.haigaiapp.cn

[Q70] 更新统计信息
来源：http://qw.colortex.cn

ANALYZE TABLE users;
来源：http://jb.gzmigu.cn

[Q71] 查看建表语句
来源：http://kk.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ba.bjjhwx.cn

[Q72] 查看索引
来源：http://wv.panjiajie.cn

SHOW INDEX FROM users;
来源：http://uc.hahajie.cn

[Q73] 查看表状态
来源：http://eb.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://en.muxihuayi.cn

[Q74] 强制使用索引
来源：http://wc.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ga.colortex.cn

[Q75] 日期格式化
来源：http://ul.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eb.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fd.521024.cn

[Q76] 按天统计
来源：http://jp.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://te.lnxyls.cn

[Q77] 时间加减
来源：http://cz.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ra.bookmarksfly.cn

[Q78] 当前时间
来源：http://ff.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qn.huanxung.cn

[Q79] 字符串拼接
来源：http://py.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tb.asd995.cn

[Q80] 字符串截取
来源：http://ai.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ei.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://xt.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mr.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://jw.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xx.haigaiapp.cn

[Q83] 大小写转换
来源：http://cx.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kt.hahajie.cn

[Q84] 去除首尾空格
来源：http://bo.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://nh.yuexingan06.cn

[Q85] 数值取整
来源：http://fe.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ou.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://ce.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kz.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://iu.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zv.521024.cn

[Q88] 行转列（条件聚合）
来源：http://zw.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ld.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ju.asd995.cn

[Q89] 判断表是否存在
来源：http://rk.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dw.huanxung.cn

[Q90] 生成序号列
来源：http://ir.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tr.szxytkj.cn

================================================================================
来源：http://ml.bookmarksfly.cn

R. Bash 专题
来源：http://lv.yuntaijiaju.cn

================================================================================
来源：http://yb.szxytkj.cn

[R01] shebang 与严格模式
来源：http://yn.jctech888.com.cn

#!/usr/bin/env bash
来源：http://dh.colortex.cn

set -euo pipefail
来源：http://gc.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://vk.9csxet.cn

name="Tom"; echo "$name"
来源：http://na.huixinmuqiang.cn

[R03] 只读变量
来源：http://lv.colortex.cn

readonly PI=3.14
来源：http://je.hahajie.cn

[R04] 位置参数
来源：http://aa.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bg.jianghongdianzi.cn

[R05] 参数默认值
来源：http://cr.huanxung.cn

name="${1:-default}"
来源：http://qy.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://ma.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yt.nszjky.cn

[R07] if 判断文件
来源：http://im.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mf.hnjuh.cn

[R08] 数值比较
来源：http://xe.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sl.panjiajie.cn

[R09] 字符串比较
来源：http://yk.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rb.jctech888.com.cn

[R10] 正则匹配
来源：http://co.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qi.szsharing.cn

[R11] case 多分支
来源：http://wp.bjjhwx.cn


<!-- 参考信息 -->
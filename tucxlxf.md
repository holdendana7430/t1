代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xh.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xa.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bl.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fo.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uv.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://le.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://po.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ou.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://co.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jz.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sf.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ck.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dl.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gn.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ap.panjiajie.cn

[P04] 求长度
来源：http://he.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bi.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qk.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ez.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qb.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://hv.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://xw.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://om.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rt.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://if.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ao.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bj.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sj.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pv.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ix.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ir.gzmigu.cn

Ruby: a == b
来源：http://ya.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yf.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zw.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cy.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://cr.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zr.nicolike.cn

TS:   if (x == null) {}
来源：http://ks.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ba.yuexingan06.cn

Go:   if x == nil {}
来源：http://qn.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ch.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://jw.huixiangedu.cn

[P07] 防抖与节流
来源：http://re.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ey.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://ag.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ht.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://of.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://um.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nu.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lk.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bh.colortex.cn

[P08] 处理浮点精度问题
来源：http://pw.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bc.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ws.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wx.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hj.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sz.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oj.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jw.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ba.colortex.cn

================================================================================
来源：http://pc.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yt.shtwfgs.cn

================================================================================
来源：http://ga.hnjuh.cn

[Q01] 创建表
来源：http://db.muxihuayi.cn

CREATE TABLE users (
来源：http://qu.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vt.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://mb.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://so.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wz.bookmarksfly.cn

);
来源：http://oe.szsharing.cn

[Q02] 创建带外键的表
来源：http://qz.szsharing.cn

CREATE TABLE orders (
来源：http://vz.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qa.nicolike.cn

user_id INT NOT NULL,
来源：http://fk.nicolike.cn

amount DECIMAL(10, 2),
来源：http://cd.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qp.jianghongdianzi.cn

);
来源：http://vb.yuntaijiaju.cn

[Q03] 增加列
来源：http://qa.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ut.gzmigu.cn

[Q04] 修改列类型
来源：http://sr.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pl.wgjwhj.cn

[Q05] 重命名列
来源：http://ga.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dd.bjjhwx.cn

[Q06] 删除列
来源：http://np.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rd.jianghongdianzi.cn

[Q07] 删除表
来源：http://bh.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://rc.9csxet.cn

[Q08] 创建普通索引
来源：http://ou.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gp.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://bo.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pz.gzmigu.cn

[Q10] 插入单行
来源：http://if.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pg.panjiajie.cn

[Q11] 一次插入多行
来源：http://jy.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xt.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://or.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://by.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sd.shxzukj.cn

[Q13] 忽略重复插入
来源：http://ok.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://em.521024.cn

[Q14] 存在则更新（upsert）
来源：http://lt.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wy.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lo.muxihuayi.cn

[Q15] 查询全部
来源：http://ra.shtwfgs.cn

SELECT * FROM users;
来源：http://vm.szxytkj.cn

[Q16] 查询指定列
来源：http://hj.haigaiapp.cn

SELECT id, name FROM users;
来源：http://jr.521024.cn

[Q17] 条件查询
来源：http://ge.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kw.haigaiapp.cn

[Q18] 模糊匹配
来源：http://jw.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ob.521024.cn

[Q19] 范围查询
来源：http://wq.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ta.asd995.cn

[Q20] IN 列表
来源：http://nl.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mw.panjiajie.cn

[Q21] 空值判断
来源：http://uu.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xw.yuntaijiaju.cn

[Q22] 排序
来源：http://kf.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fy.jianghongdianzi.cn

[Q23] 分页
来源：http://tr.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sk.haigaiapp.cn

[Q24] 去重
来源：http://lv.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://of.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://vh.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dt.wgjwhj.cn

[Q26] 计数
来源：http://do.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://ar.huixiangedu.cn

[Q27] 条件计数
来源：http://jj.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cv.hahajie.cn

[Q28] 求和与平均
来源：http://oq.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qt.lnxyls.cn

[Q29] 最大最小值
来源：http://un.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://at.huixinmuqiang.cn

[Q30] 分组统计
来源：http://lh.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eh.jctech888.com.cn

[Q31] 分组后过滤
来源：http://qq.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jf.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://wq.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jd.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hx.9csxet.cn

[Q33] 多列分组
来源：http://yz.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cc.newstarts.cn

[Q34] 每组取第一条
来源：http://ph.haigaiapp.cn

SELECT * FROM (
来源：http://vc.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://so.nicolike.cn

) t WHERE rn = 1;
来源：http://rt.bookmarksfly.cn

[Q35] 内连接
来源：http://ci.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rp.jianghongdianzi.cn

[Q36] 左连接
来源：http://vo.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://re.shxzskj.cn

[Q37] 右连接
来源：http://ku.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ll.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rf.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ij.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://mh.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sq.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ly.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ug.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pa.yuntaijiaju.cn

[Q41] 多表连接
来源：http://bo.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sp.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://mh.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://ce.asd995.cn

[Q42] 连接条件附加过滤
来源：http://nt.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://qb.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mm.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://bt.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xx.521024.cn

[Q44] IN 子查询
来源：http://lx.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gg.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://cc.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ko.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zo.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kw.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ho.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jx.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://os.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vf.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://ie.asd995.cn

[Q49] 更新单行
来源：http://cl.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xv.yuntaijiaju.cn

[Q50] 批量更新
来源：http://xi.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qw.lnxyls.cn

[Q51] 用子查询更新
来源：http://ks.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ay.chemitech.net.cn

[Q52] 删除指定行
来源：http://mg.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://nk.huixiangedu.cn

[Q53] 按条件删除
来源：http://pr.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ha.huixiangedu.cn

[Q54] 清空表
来源：http://ju.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://uc.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://an.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://no.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://rt.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kc.shxzskj.cn

[Q57] 行号
来源：http://cf.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kv.shxzskj.cn

[Q58] 累计求和
来源：http://ge.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://be.wgjwhj.cn

[Q59] 分组内累计
来源：http://dg.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hj.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://hq.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wc.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://to.nszjky.cn

[Q61] 移动平均
来源：http://wq.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pb.hahajie.cn

[Q62] 分组占比
来源：http://zl.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qk.wgjwhj.cn

[Q63] 开启事务
来源：http://ov.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gk.hahajie.cn

[Q64] 提交事务
来源：http://cf.jctech888.com.cn

COMMIT;
来源：http://oj.chemitech.net.cn

[Q65] 回滚事务
来源：http://ja.yuntaijiaju.cn

ROLLBACK;
来源：http://yt.yuexingan06.cn

[Q66] 行锁查询
来源：http://nw.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gl.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://yz.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ci.jctech888.com.cn

[Q68] 保存点
来源：http://gu.nszjky.cn

SAVEPOINT sp1;
来源：http://lc.colortex.cn

ROLLBACK TO sp1;
来源：http://wx.521024.cn

[Q69] 查看执行计划
来源：http://ah.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gg.shxzukj.cn

[Q70] 更新统计信息
来源：http://kc.panjiajie.cn

ANALYZE TABLE users;
来源：http://uq.asd995.cn

[Q71] 查看建表语句
来源：http://qo.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fl.jctech888.com.cn

[Q72] 查看索引
来源：http://um.shxzskj.cn

SHOW INDEX FROM users;
来源：http://gh.bjjhwx.cn

[Q73] 查看表状态
来源：http://hp.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dz.hahajie.cn

[Q74] 强制使用索引
来源：http://nv.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cn.hahajie.cn

[Q75] 日期格式化
来源：http://zw.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sj.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kl.wgjwhj.cn

[Q76] 按天统计
来源：http://oj.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yg.yuexingan06.cn

[Q77] 时间加减
来源：http://nu.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ct.gzmigu.cn

[Q78] 当前时间
来源：http://ol.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mf.hahajie.cn

[Q79] 字符串拼接
来源：http://fg.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tk.lnxyls.cn

[Q80] 字符串截取
来源：http://vd.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wc.hnjuh.cn

[Q81] 字符串替换
来源：http://pi.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ht.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://rk.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mq.lnxyls.cn

[Q83] 大小写转换
来源：http://cb.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hh.szsharing.cn

[Q84] 去除首尾空格
来源：http://el.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://tr.wgjwhj.cn

[Q85] 数值取整
来源：http://nq.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kl.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://xp.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ew.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://lm.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mm.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://fn.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bm.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://od.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://hc.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://td.panjiajie.cn

[Q90] 生成序号列
来源：http://mc.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nm.9csxet.cn

================================================================================
来源：http://mn.asd995.cn

R. Bash 专题
来源：http://ve.shtwfgs.cn

================================================================================
来源：http://ad.hahajie.cn

[R01] shebang 与严格模式
来源：http://mu.huanxung.cn

#!/usr/bin/env bash
来源：http://fc.shtwfgs.cn

set -euo pipefail
来源：http://fp.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://te.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://cy.9csxet.cn

[R03] 只读变量
来源：http://xp.szsharing.cn

readonly PI=3.14
来源：http://yc.bjjhwx.cn

[R04] 位置参数
来源：http://vr.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ff.huanxung.cn

[R05] 参数默认值
来源：http://ep.wgjwhj.cn

name="${1:-default}"
来源：http://rf.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://cl.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cs.colortex.cn

[R07] if 判断文件
来源：http://bd.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ps.gzmigu.cn

[R08] 数值比较
来源：http://uw.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ze.lnxyls.cn

[R09] 字符串比较
来源：http://zn.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pt.lnxyls.cn

[R10] 正则匹配
来源：http://ae.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zu.panjiajie.cn

[R11] case 多分支
来源：http://uc.shtwfgs.cn

case "$1" in
来源：http://wh.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://km.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://cr.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://yr.huixinmuqiang.cn

esac
来源：http://la.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://cu.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://xv.huanxung.cn

[R13] for 计数循环
来源：http://lh.521024.cn


<!-- 参考信息 -->
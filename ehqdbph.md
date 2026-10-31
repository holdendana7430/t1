代发 wailian999

TS:   crypto.randomUUID()
来源：http://ec.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://hq.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://qt.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://iz.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://lg.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://br.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://in.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://um.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xb.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pf.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://td.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ud.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vc.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pa.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://gm.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ks.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nr.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qw.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tt.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bo.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yb.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cy.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dh.bookmarksfly.cn

[P04] 求长度
来源：http://ot.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lm.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eu.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gj.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jf.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://py.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://if.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://me.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nm.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://mh.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ko.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sf.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xm.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mq.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fd.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yh.jianghongdianzi.cn

Ruby: a == b
来源：http://tj.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ws.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ck.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rm.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://gl.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://to.jctech888.com.cn

TS:   if (x == null) {}
来源：http://gi.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pz.chemitech.net.cn

Go:   if x == nil {}
来源：http://dx.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yo.nszjky.cn

C#:   if (x is null) {}
来源：http://an.shtwfgs.cn

[P07] 防抖与节流
来源：http://as.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://px.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://hk.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ix.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vw.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fi.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vn.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yd.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pw.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://ty.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ip.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yk.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pc.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uh.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ba.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://px.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://my.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vk.newstarts.cn

================================================================================
来源：http://bb.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pg.haigaiapp.cn

================================================================================
来源：http://ta.jctech888.com.cn

[Q01] 创建表
来源：http://hl.shtwfgs.cn

CREATE TABLE users (
来源：http://rx.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hq.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://xl.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://yh.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bh.jctech888.com.cn

);
来源：http://cu.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://af.yuexingan06.cn

CREATE TABLE orders (
来源：http://vw.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qx.9csxet.cn

user_id INT NOT NULL,
来源：http://en.nszjky.cn

amount DECIMAL(10, 2),
来源：http://mw.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pq.muxihuayi.cn

);
来源：http://zc.huixinmuqiang.cn

[Q03] 增加列
来源：http://wv.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://as.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://hw.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bf.lnxyls.cn

[Q05] 重命名列
来源：http://eb.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tp.9csxet.cn

[Q06] 删除列
来源：http://zu.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lk.hahajie.cn

[Q07] 删除表
来源：http://cw.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://ns.muxihuayi.cn

[Q08] 创建普通索引
来源：http://qu.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wu.shxzukj.cn

[Q09] 创建唯一索引
来源：http://yq.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sh.szsharing.cn

[Q10] 插入单行
来源：http://bo.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wj.hnjuh.cn

[Q11] 一次插入多行
来源：http://jw.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wc.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://ox.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gw.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hh.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://zx.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vh.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://rc.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vf.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://la.yuexingan06.cn

[Q15] 查询全部
来源：http://lw.lnxyls.cn

SELECT * FROM users;
来源：http://bo.gzmigu.cn

[Q16] 查询指定列
来源：http://qg.hahajie.cn

SELECT id, name FROM users;
来源：http://uz.muxihuayi.cn

[Q17] 条件查询
来源：http://jx.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ds.panjiajie.cn

[Q18] 模糊匹配
来源：http://ft.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dm.bookmarksfly.cn

[Q19] 范围查询
来源：http://uq.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://le.lnxyls.cn

[Q20] IN 列表
来源：http://wu.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vu.huanxung.cn

[Q21] 空值判断
来源：http://zf.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lf.newstarts.cn

[Q22] 排序
来源：http://tl.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wo.haigaiapp.cn

[Q23] 分页
来源：http://rm.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zb.shxzukj.cn

[Q24] 去重
来源：http://xc.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ou.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://bl.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cc.yuexingan06.cn

[Q26] 计数
来源：http://gq.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://us.jctech888.com.cn

[Q27] 条件计数
来源：http://zj.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fz.huixiangedu.cn

[Q28] 求和与平均
来源：http://yd.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nl.lnxyls.cn

[Q29] 最大最小值
来源：http://ab.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gi.yuntaijiaju.cn

[Q30] 分组统计
来源：http://zn.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ln.nszjky.cn

[Q31] 分组后过滤
来源：http://fb.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dp.huanxung.cn

[Q32] 分组拼接字符串
来源：http://sm.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zf.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wc.yuexingan06.cn

[Q33] 多列分组
来源：http://rz.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jp.colortex.cn

[Q34] 每组取第一条
来源：http://zu.bjjhwx.cn

SELECT * FROM (
来源：http://di.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nh.hnjuh.cn

) t WHERE rn = 1;
来源：http://jy.521024.cn

[Q35] 内连接
来源：http://cu.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://if.huixinmuqiang.cn

[Q36] 左连接
来源：http://tf.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dh.szsharing.cn

[Q37] 右连接
来源：http://ei.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ma.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ba.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zs.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://mn.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gl.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cn.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://al.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cp.9csxet.cn

[Q41] 多表连接
来源：http://th.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zx.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://nm.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://xl.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://uy.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://gh.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vj.shxzskj.cn

[Q43] 标量子查询
来源：http://kz.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aa.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://zr.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xd.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ry.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ok.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cg.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ci.huixiangedu.cn

[Q47] 与平均值比较
来源：http://fw.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ml.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://zz.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sf.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://kb.nicolike.cn

[Q49] 更新单行
来源：http://fy.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wo.szxytkj.cn

[Q50] 批量更新
来源：http://uo.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ic.nszjky.cn

[Q51] 用子查询更新
来源：http://ew.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://up.jctech888.com.cn

[Q52] 删除指定行
来源：http://ct.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://mk.shxzskj.cn

[Q53] 按条件删除
来源：http://sr.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bl.nicolike.cn

[Q54] 清空表
来源：http://cj.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ey.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://bo.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rm.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://gl.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hh.chemitech.net.cn

[Q57] 行号
来源：http://ir.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://op.hahajie.cn

[Q58] 累计求和
来源：http://os.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aw.haigaiapp.cn

[Q59] 分组内累计
来源：http://am.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hl.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://mz.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://at.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ym.wgjwhj.cn

[Q61] 移动平均
来源：http://jn.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yz.nicolike.cn

[Q62] 分组占比
来源：http://pk.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ai.colortex.cn

[Q63] 开启事务
来源：http://fn.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sp.lnxyls.cn

[Q64] 提交事务
来源：http://nh.wgjwhj.cn

COMMIT;
来源：http://oe.huanxung.cn

[Q65] 回滚事务
来源：http://ng.muxihuayi.cn

ROLLBACK;
来源：http://nj.nszjky.cn

[Q66] 行锁查询
来源：http://ro.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ez.colortex.cn

[Q67] 设置隔离级别
来源：http://sv.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nt.shtwfgs.cn

[Q68] 保存点
来源：http://vi.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://mn.shxzukj.cn

ROLLBACK TO sp1;
来源：http://xi.muxihuayi.cn

[Q69] 查看执行计划
来源：http://ej.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wz.nszjky.cn

[Q70] 更新统计信息
来源：http://rb.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://gf.colortex.cn

[Q71] 查看建表语句
来源：http://pa.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vw.bjjhwx.cn

[Q72] 查看索引
来源：http://mh.shxzskj.cn

SHOW INDEX FROM users;
来源：http://uj.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://ro.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nj.jctech888.com.cn

[Q74] 强制使用索引
来源：http://sl.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tu.szsharing.cn

[Q75] 日期格式化
来源：http://dc.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iu.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cs.haigaiapp.cn

[Q76] 按天统计
来源：http://sw.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mb.chemitech.net.cn

[Q77] 时间加减
来源：http://jp.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ln.panjiajie.cn

[Q78] 当前时间
来源：http://fh.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ij.newstarts.cn

[Q79] 字符串拼接
来源：http://hy.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kz.521024.cn

[Q80] 字符串截取
来源：http://ii.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kv.lnxyls.cn

[Q81] 字符串替换
来源：http://sq.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mn.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://oa.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ig.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://ju.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ss.shxzskj.cn

[Q84] 去除首尾空格
来源：http://en.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://ju.szxytkj.cn

[Q85] 数值取整
来源：http://pz.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eb.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://vj.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gd.9csxet.cn

[Q87] JSON 字段做条件
来源：http://yt.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ud.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://yc.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://na.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sv.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://ax.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ta.nszjky.cn

[Q90] 生成序号列
来源：http://pw.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lq.hnjuh.cn

================================================================================
来源：http://wt.muxihuayi.cn

R. Bash 专题
来源：http://xi.asd995.cn

================================================================================
来源：http://ch.szxytkj.cn

[R01] shebang 与严格模式
来源：http://os.muxihuayi.cn

#!/usr/bin/env bash
来源：http://oe.shxzskj.cn

set -euo pipefail
来源：http://zh.lnxyls.cn

[R02] 变量赋值与使用
来源：http://of.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://db.huixiangedu.cn

[R03] 只读变量
来源：http://nt.nszjky.cn

readonly PI=3.14
来源：http://wq.9csxet.cn

[R04] 位置参数
来源：http://pg.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zx.chemitech.net.cn

[R05] 参数默认值
来源：http://nm.huixinmuqiang.cn

name="${1:-default}"
来源：http://lq.gzmigu.cn

[R06] 判断命令是否存在
来源：http://yn.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ey.yuntaijiaju.cn

[R07] if 判断文件
来源：http://tk.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ri.bjjhwx.cn

[R08] 数值比较
来源：http://wv.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wf.jianghongdianzi.cn

[R09] 字符串比较
来源：http://uh.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bs.shxzukj.cn

[R10] 正则匹配
来源：http://en.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qd.521024.cn

[R11] case 多分支
来源：http://pm.huixinmuqiang.cn


<!-- 参考信息 -->
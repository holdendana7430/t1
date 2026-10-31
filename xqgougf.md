代发 wailian999

C#:   Parallel.For
来源：http://hn.hnjuh.cn

================================================================================
来源：http://yx.colortex.cn

P. 常用工具函数
来源：http://ta.bjjhwx.cn

================================================================================
来源：http://ql.jctech888.com.cn

[P01] 生成 UUID
来源：http://ks.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://fc.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fh.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://bd.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://uw.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://qt.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://em.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://ut.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://un.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://yg.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pq.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nk.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dt.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pb.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kc.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qb.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yl.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pt.shxzukj.cn

[P03] 生成短随机字符串
来源：http://pj.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xl.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oo.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xu.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qm.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fm.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cn.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fb.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vv.muxihuayi.cn

[P04] 求长度
来源：http://ai.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mp.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gw.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ku.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hv.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://ni.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://df.szxytkj.cn

Ruby: x.length;  x.size
来源：http://vj.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zu.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ol.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ex.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mj.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gx.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rh.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kc.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sb.huanxung.cn

Ruby: a == b
来源：http://yy.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://th.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aj.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kk.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://sh.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vm.szsharing.cn

TS:   if (x == null) {}
来源：http://fk.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ek.wgjwhj.cn

Go:   if x == nil {}
来源：http://qu.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://du.hnjuh.cn

C#:   if (x is null) {}
来源：http://dp.newstarts.cn

[P07] 防抖与节流
来源：http://bi.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gv.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://ky.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://or.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ix.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xb.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dk.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xb.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fr.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://yh.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://re.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fq.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aa.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://io.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zl.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kh.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bj.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ou.hahajie.cn

================================================================================
来源：http://mb.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://za.nicolike.cn

================================================================================
来源：http://hy.szxytkj.cn

[Q01] 创建表
来源：http://cb.shtwfgs.cn

CREATE TABLE users (
来源：http://kq.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fw.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://mk.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://wd.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://av.yuntaijiaju.cn

);
来源：http://rh.nszjky.cn

[Q02] 创建带外键的表
来源：http://iv.szsharing.cn

CREATE TABLE orders (
来源：http://yv.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://bw.nszjky.cn

amount DECIMAL(10, 2),
来源：http://lw.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rx.lnxyls.cn

);
来源：http://ts.chemitech.net.cn

[Q03] 增加列
来源：http://pm.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kn.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://ie.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://za.shxzukj.cn

[Q05] 重命名列
来源：http://as.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ns.haigaiapp.cn

[Q06] 删除列
来源：http://ma.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pt.szsharing.cn

[Q07] 删除表
来源：http://wf.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://hg.asd995.cn

[Q08] 创建普通索引
来源：http://dw.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sp.hahajie.cn

[Q09] 创建唯一索引
来源：http://vq.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wq.colortex.cn

[Q10] 插入单行
来源：http://gn.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vz.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://al.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ba.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://fx.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fk.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mf.hnjuh.cn

[Q13] 忽略重复插入
来源：http://ik.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hk.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://uc.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ro.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hf.colortex.cn

[Q15] 查询全部
来源：http://tl.jianghongdianzi.cn

SELECT * FROM users;
来源：http://ax.wgjwhj.cn

[Q16] 查询指定列
来源：http://zx.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://to.wgjwhj.cn

[Q17] 条件查询
来源：http://fb.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://et.huixiangedu.cn

[Q18] 模糊匹配
来源：http://wy.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ts.jianghongdianzi.cn

[Q19] 范围查询
来源：http://on.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zo.muxihuayi.cn

[Q20] IN 列表
来源：http://hg.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://md.9csxet.cn

[Q21] 空值判断
来源：http://rv.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vv.szsharing.cn

[Q22] 排序
来源：http://ri.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ib.panjiajie.cn

[Q23] 分页
来源：http://fe.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ao.9csxet.cn

[Q24] 去重
来源：http://js.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://jz.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://zq.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://op.yuntaijiaju.cn

[Q26] 计数
来源：http://up.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://is.haigaiapp.cn

[Q27] 条件计数
来源：http://hb.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eu.shxzukj.cn

[Q28] 求和与平均
来源：http://lw.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://it.nszjky.cn

[Q29] 最大最小值
来源：http://up.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qf.hahajie.cn

[Q30] 分组统计
来源：http://fs.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ga.panjiajie.cn

[Q31] 分组后过滤
来源：http://hz.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://du.newstarts.cn

[Q32] 分组拼接字符串
来源：http://ej.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ga.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xf.9csxet.cn

[Q33] 多列分组
来源：http://hu.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jz.panjiajie.cn

[Q34] 每组取第一条
来源：http://qg.huanxung.cn

SELECT * FROM (
来源：http://uh.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pg.hnjuh.cn

) t WHERE rn = 1;
来源：http://ox.panjiajie.cn

[Q35] 内连接
来源：http://sz.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ue.nszjky.cn

[Q36] 左连接
来源：http://at.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xc.hahajie.cn

[Q37] 右连接
来源：http://xy.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gq.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://by.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tg.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://ju.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://im.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hf.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://il.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yc.shxzukj.cn

[Q41] 多表连接
来源：http://bt.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zp.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://ce.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vh.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://jh.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://ei.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://do.haigaiapp.cn

[Q43] 标量子查询
来源：http://yf.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://en.nszjky.cn

[Q44] IN 子查询
来源：http://df.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dj.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://cw.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mr.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vk.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yp.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://rr.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ie.colortex.cn

[Q48] CTE 公用表表达式
来源：http://jc.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jx.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://rv.shxzskj.cn

[Q49] 更新单行
来源：http://vo.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cl.yuexingan06.cn

[Q50] 批量更新
来源：http://qx.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kh.nszjky.cn

[Q51] 用子查询更新
来源：http://nx.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jb.hnjuh.cn

[Q52] 删除指定行
来源：http://ta.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://kq.panjiajie.cn

[Q53] 按条件删除
来源：http://mk.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://he.szsharing.cn

[Q54] 清空表
来源：http://qf.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://aa.hahajie.cn

[Q55] 排名（并列占位）
来源：http://oq.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://za.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://ir.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nz.newstarts.cn

[Q57] 行号
来源：http://ky.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ig.huixiangedu.cn

[Q58] 累计求和
来源：http://jm.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hp.bookmarksfly.cn

[Q59] 分组内累计
来源：http://mo.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ao.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://si.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vc.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xf.shtwfgs.cn

[Q61] 移动平均
来源：http://oq.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ht.jianghongdianzi.cn

[Q62] 分组占比
来源：http://wu.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lo.gzmigu.cn

[Q63] 开启事务
来源：http://fg.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wr.chemitech.net.cn

[Q64] 提交事务
来源：http://yg.huanxung.cn

COMMIT;
来源：http://lt.szsharing.cn

[Q65] 回滚事务
来源：http://ap.hahajie.cn

ROLLBACK;
来源：http://xh.bjjhwx.cn

[Q66] 行锁查询
来源：http://bg.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vf.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://jy.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wb.huanxung.cn

[Q68] 保存点
来源：http://pj.muxihuayi.cn

SAVEPOINT sp1;
来源：http://bo.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://xz.panjiajie.cn

[Q69] 查看执行计划
来源：http://lh.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dr.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://lg.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://nq.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://nz.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ml.bookmarksfly.cn

[Q72] 查看索引
来源：http://vh.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://tb.colortex.cn

[Q73] 查看表状态
来源：http://qp.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ji.yuexingan06.cn

[Q74] 强制使用索引
来源：http://in.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ks.asd995.cn

[Q75] 日期格式化
来源：http://wu.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cc.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gd.shxzukj.cn

[Q76] 按天统计
来源：http://bg.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sz.bjjhwx.cn

[Q77] 时间加减
来源：http://go.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sv.yuexingan06.cn

[Q78] 当前时间
来源：http://nn.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sh.panjiajie.cn

[Q79] 字符串拼接
来源：http://jl.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dm.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://ik.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cx.shtwfgs.cn

[Q81] 字符串替换
来源：http://jv.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yi.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://dd.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fs.chemitech.net.cn

[Q83] 大小写转换
来源：http://wh.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rz.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://yu.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://jr.asd995.cn

[Q85] 数值取整
来源：http://py.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dp.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://zy.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rb.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://sk.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://se.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://af.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wq.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sk.nicolike.cn

[Q89] 判断表是否存在
来源：http://sy.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ki.nszjky.cn

[Q90] 生成序号列
来源：http://sq.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://me.bookmarksfly.cn

================================================================================
来源：http://sz.panjiajie.cn

R. Bash 专题
来源：http://vg.gzmigu.cn

================================================================================
来源：http://nx.panjiajie.cn

[R01] shebang 与严格模式
来源：http://lq.hnjuh.cn

#!/usr/bin/env bash
来源：http://jr.9csxet.cn

set -euo pipefail
来源：http://ce.nszjky.cn

[R02] 变量赋值与使用
来源：http://al.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://js.wgjwhj.cn

[R03] 只读变量
来源：http://xx.bookmarksfly.cn

readonly PI=3.14
来源：http://pa.huixinmuqiang.cn

[R04] 位置参数
来源：http://gh.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mi.szxytkj.cn

[R05] 参数默认值
来源：http://ox.nszjky.cn

name="${1:-default}"
来源：http://dn.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://py.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pg.huixiangedu.cn

[R07] if 判断文件
来源：http://be.shxzskj.cn


<!-- 参考信息 -->
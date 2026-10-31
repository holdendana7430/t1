代发 wailian999

TS:   // child_process / cluster 模块
来源：http://sj.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yb.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bp.9csxet.cn

Ruby: // fork 块
来源：http://cw.lnxyls.cn

C#:   Parallel.For
来源：http://sb.hahajie.cn

================================================================================
来源：http://xb.panjiajie.cn

P. 常用工具函数
来源：http://re.panjiajie.cn

================================================================================
来源：http://wk.9csxet.cn

[P01] 生成 UUID
来源：http://aa.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://nt.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zf.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://rc.nszjky.cn

TS:   crypto.randomUUID()
来源：http://qh.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://nf.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://vd.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://uz.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://tt.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://gw.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://et.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qy.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fi.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ra.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jc.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yi.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jw.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jm.gzmigu.cn

[P03] 生成短随机字符串
来源：http://yf.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://af.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xj.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ee.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ep.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gc.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cl.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oc.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://an.chemitech.net.cn

[P04] 求长度
来源：http://qz.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ne.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zt.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dz.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://am.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://qm.521024.cn

Go:   len(arr);  len(m)
来源：http://ge.nicolike.cn

Ruby: x.length;  x.size
来源：http://rf.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fb.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://jo.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://me.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qe.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bx.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kb.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iu.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yb.shxzskj.cn

Ruby: a == b
来源：http://ar.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hy.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cd.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zz.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://ge.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wh.szsharing.cn

TS:   if (x == null) {}
来源：http://mk.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ne.bjjhwx.cn

Go:   if x == nil {}
来源：http://jq.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xt.bjjhwx.cn

C#:   if (x is null) {}
来源：http://ou.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ya.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hq.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://bq.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qg.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oe.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://me.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lw.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zb.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://im.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://gg.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qv.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uo.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://el.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hx.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oq.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qm.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zr.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://me.colortex.cn

================================================================================
来源：http://da.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jb.bookmarksfly.cn

================================================================================
来源：http://se.9csxet.cn

[Q01] 创建表
来源：http://cp.yuexingan06.cn

CREATE TABLE users (
来源：http://wp.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ee.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://nc.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://dv.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mv.nicolike.cn

);
来源：http://lw.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://su.jctech888.com.cn

CREATE TABLE orders (
来源：http://lc.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ju.shxzukj.cn

user_id INT NOT NULL,
来源：http://vw.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://db.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lh.haigaiapp.cn

);
来源：http://xv.wgjwhj.cn

[Q03] 增加列
来源：http://wp.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ct.chemitech.net.cn

[Q04] 修改列类型
来源：http://lq.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wo.yuexingan06.cn

[Q05] 重命名列
来源：http://hn.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lv.shxzskj.cn

[Q06] 删除列
来源：http://km.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zb.haigaiapp.cn

[Q07] 删除表
来源：http://yo.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://us.haigaiapp.cn

[Q08] 创建普通索引
来源：http://rw.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bx.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://qg.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ei.szsharing.cn

[Q10] 插入单行
来源：http://et.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xz.panjiajie.cn

[Q11] 一次插入多行
来源：http://jy.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lw.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://yx.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nt.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rv.9csxet.cn

[Q13] 忽略重复插入
来源：http://wt.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://od.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://fx.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bd.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ux.szxytkj.cn

[Q15] 查询全部
来源：http://ee.muxihuayi.cn

SELECT * FROM users;
来源：http://fp.bookmarksfly.cn

[Q16] 查询指定列
来源：http://sx.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://ji.newstarts.cn

[Q17] 条件查询
来源：http://gx.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jc.huanxung.cn

[Q18] 模糊匹配
来源：http://um.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zs.asd995.cn

[Q19] 范围查询
来源：http://ib.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hj.jianghongdianzi.cn

[Q20] IN 列表
来源：http://jk.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fz.chemitech.net.cn

[Q21] 空值判断
来源：http://fk.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lu.colortex.cn

[Q22] 排序
来源：http://ec.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tb.bjjhwx.cn

[Q23] 分页
来源：http://zt.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://av.shxzukj.cn

[Q24] 去重
来源：http://ld.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://di.colortex.cn

[Q25] 只取前 N 条
来源：http://mi.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jf.gzmigu.cn

[Q26] 计数
来源：http://fx.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ak.panjiajie.cn

[Q27] 条件计数
来源：http://kj.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://di.bjjhwx.cn

[Q28] 求和与平均
来源：http://ti.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jo.chemitech.net.cn

[Q29] 最大最小值
来源：http://dy.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kz.jctech888.com.cn

[Q30] 分组统计
来源：http://iy.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lt.muxihuayi.cn

[Q31] 分组后过滤
来源：http://bu.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ek.asd995.cn

[Q32] 分组拼接字符串
来源：http://gq.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zj.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bk.wgjwhj.cn

[Q33] 多列分组
来源：http://kc.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kt.wgjwhj.cn

[Q34] 每组取第一条
来源：http://wx.haigaiapp.cn

SELECT * FROM (
来源：http://tm.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tl.szsharing.cn

) t WHERE rn = 1;
来源：http://bb.huanxung.cn

[Q35] 内连接
来源：http://pd.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://um.hnjuh.cn

[Q36] 左连接
来源：http://er.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jl.newstarts.cn

[Q37] 右连接
来源：http://gr.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ho.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hv.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fl.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://mj.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zz.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://il.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://se.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oh.panjiajie.cn

[Q41] 多表连接
来源：http://uv.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wx.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://wt.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://os.colortex.cn

[Q42] 连接条件附加过滤
来源：http://ti.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://ey.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://az.panjiajie.cn

[Q43] 标量子查询
来源：http://rg.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vm.asd995.cn

[Q44] IN 子查询
来源：http://js.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qu.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://ll.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rt.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cx.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rk.9csxet.cn

[Q47] 与平均值比较
来源：http://mn.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yn.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://pw.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xa.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://qs.wgjwhj.cn

[Q49] 更新单行
来源：http://xv.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xo.gzmigu.cn

[Q50] 批量更新
来源：http://qd.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zq.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://tj.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://og.colortex.cn

[Q52] 删除指定行
来源：http://uy.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://hi.jctech888.com.cn

[Q53] 按条件删除
来源：http://ja.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nd.hahajie.cn

[Q54] 清空表
来源：http://yi.521024.cn

TRUNCATE TABLE logs;
来源：http://em.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://on.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wz.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://tq.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rl.panjiajie.cn

[Q57] 行号
来源：http://ll.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ew.huanxung.cn

[Q58] 累计求和
来源：http://oj.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bk.haigaiapp.cn

[Q59] 分组内累计
来源：http://bl.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qu.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://jl.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ab.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lq.asd995.cn

[Q61] 移动平均
来源：http://zs.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vx.hahajie.cn

[Q62] 分组占比
来源：http://oh.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cp.panjiajie.cn

[Q63] 开启事务
来源：http://zv.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rr.yuntaijiaju.cn

[Q64] 提交事务
来源：http://td.chemitech.net.cn

COMMIT;
来源：http://om.chemitech.net.cn

[Q65] 回滚事务
来源：http://ws.szxytkj.cn

ROLLBACK;
来源：http://wl.asd995.cn

[Q66] 行锁查询
来源：http://cf.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fb.lnxyls.cn

[Q67] 设置隔离级别
来源：http://dl.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kf.gzmigu.cn

[Q68] 保存点
来源：http://mg.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://sp.nicolike.cn

ROLLBACK TO sp1;
来源：http://og.shtwfgs.cn

[Q69] 查看执行计划
来源：http://ot.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gt.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://pm.lnxyls.cn

ANALYZE TABLE users;
来源：http://vv.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://bf.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dc.newstarts.cn

[Q72] 查看索引
来源：http://ff.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://ta.colortex.cn

[Q73] 查看表状态
来源：http://eh.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ur.haigaiapp.cn

[Q74] 强制使用索引
来源：http://ly.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nz.bjjhwx.cn

[Q75] 日期格式化
来源：http://dr.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cz.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pt.haigaiapp.cn

[Q76] 按天统计
来源：http://cd.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nz.9csxet.cn

[Q77] 时间加减
来源：http://nj.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gw.haigaiapp.cn

[Q78] 当前时间
来源：http://ge.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://us.szsharing.cn

[Q79] 字符串拼接
来源：http://zc.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bx.szxytkj.cn

[Q80] 字符串截取
来源：http://ub.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gi.gzmigu.cn

[Q81] 字符串替换
来源：http://oz.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nf.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://vq.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ql.shtwfgs.cn

[Q83] 大小写转换
来源：http://le.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rl.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://om.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://so.chemitech.net.cn

[Q85] 数值取整
来源：http://bo.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lr.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://eq.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uh.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://rz.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kf.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://dv.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dp.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oe.nicolike.cn

[Q89] 判断表是否存在
来源：http://zx.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qd.asd995.cn

[Q90] 生成序号列
来源：http://zm.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://im.nszjky.cn

================================================================================
来源：http://ox.nszjky.cn

R. Bash 专题
来源：http://dy.newstarts.cn

================================================================================
来源：http://hk.hahajie.cn

[R01] shebang 与严格模式
来源：http://qp.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://ng.bjjhwx.cn

set -euo pipefail
来源：http://kq.hahajie.cn

[R02] 变量赋值与使用
来源：http://lb.asd995.cn

name="Tom"; echo "$name"
来源：http://el.szsharing.cn

[R03] 只读变量
来源：http://rm.yuexingan06.cn

readonly PI=3.14
来源：http://ph.521024.cn

[R04] 位置参数
来源：http://qb.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ar.lnxyls.cn

[R05] 参数默认值
来源：http://ly.nicolike.cn


<!-- 参考信息 -->
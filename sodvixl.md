代发 wailian999

TS:   crypto.randomUUID()
来源：http://gs.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://je.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://un.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://sf.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://yw.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://kb.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kd.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jf.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oi.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://km.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ng.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sg.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fm.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uu.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://xv.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bb.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fx.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gi.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jw.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jk.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ue.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rh.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xt.yuexingan06.cn

[P04] 求长度
来源：http://wa.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jz.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wv.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ng.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bl.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://pr.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://fd.colortex.cn

Ruby: x.length;  x.size
来源：http://gg.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gf.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://iy.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wb.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cy.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://th.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xl.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ls.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kr.shxzskj.cn

Ruby: a == b
来源：http://qq.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cq.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rk.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ek.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://ew.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uc.521024.cn

TS:   if (x == null) {}
来源：http://hp.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jv.huanxung.cn

Go:   if x == nil {}
来源：http://lp.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sc.muxihuayi.cn

C#:   if (x is null) {}
来源：http://fi.newstarts.cn

[P07] 防抖与节流
来源：http://qx.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qf.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://yk.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qn.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://io.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bq.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dd.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rn.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tb.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://vm.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cs.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uo.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://di.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dd.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hd.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aj.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ti.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wl.hnjuh.cn

================================================================================
来源：http://zq.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yu.chemitech.net.cn

================================================================================
来源：http://el.huanxung.cn

[Q01] 创建表
来源：http://xc.huanxung.cn

CREATE TABLE users (
来源：http://fu.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gd.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://jm.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://cj.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jo.colortex.cn

);
来源：http://bk.9csxet.cn

[Q02] 创建带外键的表
来源：http://if.huixiangedu.cn

CREATE TABLE orders (
来源：http://nx.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kp.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://ed.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://cz.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://go.haigaiapp.cn

);
来源：http://xx.521024.cn

[Q03] 增加列
来源：http://bj.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cy.hahajie.cn

[Q04] 修改列类型
来源：http://ss.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xn.huixiangedu.cn

[Q05] 重命名列
来源：http://rv.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://do.jctech888.com.cn

[Q06] 删除列
来源：http://md.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yj.huixiangedu.cn

[Q07] 删除表
来源：http://cw.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://gp.shxzukj.cn

[Q08] 创建普通索引
来源：http://pk.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pm.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://rx.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dr.muxihuayi.cn

[Q10] 插入单行
来源：http://bk.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cp.jctech888.com.cn

[Q11] 一次插入多行
来源：http://yu.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gh.colortex.cn

[Q12] 插入后取自增 ID
来源：http://bj.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eb.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pl.gzmigu.cn

[Q13] 忽略重复插入
来源：http://vo.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zo.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://ni.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tv.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wv.huixinmuqiang.cn

[Q15] 查询全部
来源：http://sd.chemitech.net.cn

SELECT * FROM users;
来源：http://ur.bookmarksfly.cn

[Q16] 查询指定列
来源：http://wk.shxzskj.cn

SELECT id, name FROM users;
来源：http://pl.wgjwhj.cn

[Q17] 条件查询
来源：http://nw.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yn.huixiangedu.cn

[Q18] 模糊匹配
来源：http://ts.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wh.szxytkj.cn

[Q19] 范围查询
来源：http://jx.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qb.haigaiapp.cn

[Q20] IN 列表
来源：http://pk.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://os.newstarts.cn

[Q21] 空值判断
来源：http://cd.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aj.521024.cn

[Q22] 排序
来源：http://sq.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pd.nszjky.cn

[Q23] 分页
来源：http://au.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vp.hnjuh.cn

[Q24] 去重
来源：http://qd.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://cl.shxzukj.cn

[Q25] 只取前 N 条
来源：http://zh.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xg.nicolike.cn

[Q26] 计数
来源：http://jx.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://yw.szxytkj.cn

[Q27] 条件计数
来源：http://xg.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://km.lnxyls.cn

[Q28] 求和与平均
来源：http://hf.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bt.nszjky.cn

[Q29] 最大最小值
来源：http://gx.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xa.haigaiapp.cn

[Q30] 分组统计
来源：http://np.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vx.szxytkj.cn

[Q31] 分组后过滤
来源：http://ft.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bu.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://ea.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qf.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jt.muxihuayi.cn

[Q33] 多列分组
来源：http://ss.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://te.lnxyls.cn

[Q34] 每组取第一条
来源：http://hn.shtwfgs.cn

SELECT * FROM (
来源：http://rq.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hs.jctech888.com.cn

) t WHERE rn = 1;
来源：http://ys.521024.cn

[Q35] 内连接
来源：http://uu.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ep.huixinmuqiang.cn

[Q36] 左连接
来源：http://kv.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jl.huixiangedu.cn

[Q37] 右连接
来源：http://ws.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jt.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ds.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qv.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://jr.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jh.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xk.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cu.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jj.lnxyls.cn

[Q41] 多表连接
来源：http://tq.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bm.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://rt.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://gm.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://cj.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ot.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yj.bjjhwx.cn

[Q43] 标量子查询
来源：http://qr.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rj.chemitech.net.cn

[Q44] IN 子查询
来源：http://ov.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ea.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://yr.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fc.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bc.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fb.asd995.cn

[Q47] 与平均值比较
来源：http://nf.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ku.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://qm.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zv.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://pn.huanxung.cn

[Q49] 更新单行
来源：http://mi.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qr.muxihuayi.cn

[Q50] 批量更新
来源：http://hs.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://np.huanxung.cn

[Q51] 用子查询更新
来源：http://cj.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oj.jctech888.com.cn

[Q52] 删除指定行
来源：http://cn.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://mf.hnjuh.cn

[Q53] 按条件删除
来源：http://uv.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ip.jctech888.com.cn

[Q54] 清空表
来源：http://uw.nicolike.cn

TRUNCATE TABLE logs;
来源：http://za.hahajie.cn

[Q55] 排名（并列占位）
来源：http://ke.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qz.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://zs.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cr.bjjhwx.cn

[Q57] 行号
来源：http://xy.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://or.chemitech.net.cn

[Q58] 累计求和
来源：http://rx.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ev.newstarts.cn

[Q59] 分组内累计
来源：http://fk.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mz.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://na.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://la.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yu.haigaiapp.cn

[Q61] 移动平均
来源：http://tx.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fy.shxzukj.cn

[Q62] 分组占比
来源：http://is.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://br.bookmarksfly.cn

[Q63] 开启事务
来源：http://wd.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tz.9csxet.cn

[Q64] 提交事务
来源：http://ba.colortex.cn

COMMIT;
来源：http://to.nicolike.cn

[Q65] 回滚事务
来源：http://pi.nszjky.cn

ROLLBACK;
来源：http://lq.bookmarksfly.cn

[Q66] 行锁查询
来源：http://hi.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ug.szxytkj.cn

[Q67] 设置隔离级别
来源：http://rs.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ji.gzmigu.cn

[Q68] 保存点
来源：http://lr.newstarts.cn

SAVEPOINT sp1;
来源：http://sp.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://kg.huanxung.cn

[Q69] 查看执行计划
来源：http://gw.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tj.hnjuh.cn

[Q70] 更新统计信息
来源：http://gv.colortex.cn

ANALYZE TABLE users;
来源：http://hx.521024.cn

[Q71] 查看建表语句
来源：http://gk.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tl.yuexingan06.cn

[Q72] 查看索引
来源：http://sy.huanxung.cn

SHOW INDEX FROM users;
来源：http://fj.gzmigu.cn

[Q73] 查看表状态
来源：http://pj.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hd.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://rf.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qe.muxihuayi.cn

[Q75] 日期格式化
来源：http://ek.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kw.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dn.haigaiapp.cn

[Q76] 按天统计
来源：http://ju.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ya.szxytkj.cn

[Q77] 时间加减
来源：http://dl.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lz.huanxung.cn

[Q78] 当前时间
来源：http://vt.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xb.hnjuh.cn

[Q79] 字符串拼接
来源：http://hl.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hx.shtwfgs.cn

[Q80] 字符串截取
来源：http://ic.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ph.huanxung.cn

[Q81] 字符串替换
来源：http://se.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pb.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://mt.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gp.szxytkj.cn

[Q83] 大小写转换
来源：http://cy.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kh.hahajie.cn

[Q84] 去除首尾空格
来源：http://bf.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://kl.shxzskj.cn

[Q85] 数值取整
来源：http://ij.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pg.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://kq.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vi.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://fn.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tt.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://yh.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://af.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xu.newstarts.cn

[Q89] 判断表是否存在
来源：http://ld.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zh.hahajie.cn

[Q90] 生成序号列
来源：http://ny.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eh.hnjuh.cn

================================================================================
来源：http://kh.shxzskj.cn

R. Bash 专题
来源：http://do.colortex.cn

================================================================================
来源：http://bk.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://qs.shtwfgs.cn

#!/usr/bin/env bash
来源：http://jy.yuexingan06.cn

set -euo pipefail
来源：http://br.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://tk.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://fl.huixiangedu.cn

[R03] 只读变量
来源：http://pa.bjjhwx.cn

readonly PI=3.14
来源：http://ca.huixinmuqiang.cn

[R04] 位置参数
来源：http://pv.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zb.yuntaijiaju.cn

[R05] 参数默认值
来源：http://au.jianghongdianzi.cn

name="${1:-default}"
来源：http://sm.colortex.cn

[R06] 判断命令是否存在
来源：http://gp.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ig.szsharing.cn

[R07] if 判断文件
来源：http://ey.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fz.haigaiapp.cn

[R08] 数值比较
来源：http://rr.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qj.yuntaijiaju.cn

[R09] 字符串比较
来源：http://sb.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://je.newstarts.cn

[R10] 正则匹配
来源：http://rb.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hi.wgjwhj.cn

[R11] case 多分支
来源：http://sz.panjiajie.cn


<!-- 参考信息 -->
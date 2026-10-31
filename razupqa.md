代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qf.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ha.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://fo.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pi.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lx.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gb.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bl.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ec.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bd.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xg.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://um.huixiangedu.cn

[P04] 求长度
来源：http://ft.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uq.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fa.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yk.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://or.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://ex.521024.cn

Go:   len(arr);  len(m)
来源：http://se.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://tw.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qp.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://zm.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bw.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cn.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pm.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tx.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jv.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qr.shxzukj.cn

Ruby: a == b
来源：http://eo.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bl.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vi.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dl.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://ly.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://my.jctech888.com.cn

TS:   if (x == null) {}
来源：http://ka.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ay.shxzukj.cn

Go:   if x == nil {}
来源：http://nv.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ms.nicolike.cn

C#:   if (x is null) {}
来源：http://ua.huixiangedu.cn

[P07] 防抖与节流
来源：http://tt.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hl.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://jp.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fh.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cs.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ye.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rl.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xs.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bt.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://dr.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ws.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cs.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oo.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sg.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bm.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mt.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aw.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yp.shtwfgs.cn

================================================================================
来源：http://gv.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wn.jctech888.com.cn

================================================================================
来源：http://zd.hnjuh.cn

[Q01] 创建表
来源：http://su.nicolike.cn

CREATE TABLE users (
来源：http://nc.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eq.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://hx.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://kp.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://py.huixinmuqiang.cn

);
来源：http://ki.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://ji.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://gy.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bb.huanxung.cn

user_id INT NOT NULL,
来源：http://js.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://jc.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ue.bookmarksfly.cn

);
来源：http://fw.9csxet.cn

[Q03] 增加列
来源：http://vr.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iy.colortex.cn

[Q04] 修改列类型
来源：http://uk.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qg.huanxung.cn

[Q05] 重命名列
来源：http://uv.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cg.huixinmuqiang.cn

[Q06] 删除列
来源：http://sn.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pn.chemitech.net.cn

[Q07] 删除表
来源：http://pe.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://av.shxzskj.cn

[Q08] 创建普通索引
来源：http://to.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vq.9csxet.cn

[Q09] 创建唯一索引
来源：http://fa.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oo.shxzukj.cn

[Q10] 插入单行
来源：http://ih.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nd.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://ai.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ar.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://cx.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xt.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sn.newstarts.cn

[Q13] 忽略重复插入
来源：http://ee.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sy.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://is.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vv.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iu.lnxyls.cn

[Q15] 查询全部
来源：http://ha.wgjwhj.cn

SELECT * FROM users;
来源：http://at.szxytkj.cn

[Q16] 查询指定列
来源：http://yd.panjiajie.cn

SELECT id, name FROM users;
来源：http://sv.9csxet.cn

[Q17] 条件查询
来源：http://bg.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://er.nszjky.cn

[Q18] 模糊匹配
来源：http://bi.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ws.chemitech.net.cn

[Q19] 范围查询
来源：http://oz.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gd.newstarts.cn

[Q20] IN 列表
来源：http://ui.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nc.chemitech.net.cn

[Q21] 空值判断
来源：http://ho.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lc.asd995.cn

[Q22] 排序
来源：http://pe.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bl.gzmigu.cn

[Q23] 分页
来源：http://zf.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oi.bookmarksfly.cn

[Q24] 去重
来源：http://lv.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://yo.colortex.cn

[Q25] 只取前 N 条
来源：http://hv.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jn.bookmarksfly.cn

[Q26] 计数
来源：http://sk.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://tg.gzmigu.cn

[Q27] 条件计数
来源：http://pq.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qm.nszjky.cn

[Q28] 求和与平均
来源：http://lj.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bz.shxzukj.cn

[Q29] 最大最小值
来源：http://ax.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aa.asd995.cn

[Q30] 分组统计
来源：http://hb.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bl.wgjwhj.cn

[Q31] 分组后过滤
来源：http://wg.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ob.nicolike.cn

[Q32] 分组拼接字符串
来源：http://ly.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zr.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zv.huixiangedu.cn

[Q33] 多列分组
来源：http://ek.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fs.gzmigu.cn

[Q34] 每组取第一条
来源：http://zb.shtwfgs.cn

SELECT * FROM (
来源：http://an.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pt.panjiajie.cn

) t WHERE rn = 1;
来源：http://qs.hahajie.cn

[Q35] 内连接
来源：http://wp.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cj.lnxyls.cn

[Q36] 左连接
来源：http://gv.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pl.bjjhwx.cn

[Q37] 右连接
来源：http://kl.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tk.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wq.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mi.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://kb.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://im.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cr.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uu.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://du.asd995.cn

[Q41] 多表连接
来源：http://cg.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wm.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://ud.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://st.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://ip.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ty.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://km.shxzskj.cn

[Q43] 标量子查询
来源：http://oy.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ii.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://pc.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ca.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://vd.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://js.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://od.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnjuh.cn

[Q47] 与平均值比较
来源：http://em.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lr.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://co.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://un.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://yy.jianghongdianzi.cn

[Q49] 更新单行
来源：http://tg.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fn.shxzskj.cn

[Q50] 批量更新
来源：http://zg.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kt.colortex.cn

[Q51] 用子查询更新
来源：http://zn.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hp.nicolike.cn

[Q52] 删除指定行
来源：http://sz.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://hq.asd995.cn

[Q53] 按条件删除
来源：http://ys.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ws.gzmigu.cn

[Q54] 清空表
来源：http://az.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://uq.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://oo.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hh.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://qr.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zo.huixiangedu.cn

[Q57] 行号
来源：http://ho.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vo.lnxyls.cn

[Q58] 累计求和
来源：http://qd.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rb.nicolike.cn

[Q59] 分组内累计
来源：http://id.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uy.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://wv.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kg.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wa.hahajie.cn

[Q61] 移动平均
来源：http://fi.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qx.9csxet.cn

[Q62] 分组占比
来源：http://vw.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jo.nszjky.cn

[Q63] 开启事务
来源：http://by.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ad.shxzskj.cn

[Q64] 提交事务
来源：http://xq.bjjhwx.cn

COMMIT;
来源：http://os.bjjhwx.cn

[Q65] 回滚事务
来源：http://oh.hahajie.cn

ROLLBACK;
来源：http://ln.nicolike.cn

[Q66] 行锁查询
来源：http://si.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cx.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://wq.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fk.hnjuh.cn

[Q68] 保存点
来源：http://st.lnxyls.cn

SAVEPOINT sp1;
来源：http://cd.nszjky.cn

ROLLBACK TO sp1;
来源：http://cl.jctech888.com.cn

[Q69] 查看执行计划
来源：http://mk.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bg.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://tf.haigaiapp.cn

ANALYZE TABLE users;
来源：http://pk.shxzskj.cn

[Q71] 查看建表语句
来源：http://cf.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gz.huixiangedu.cn

[Q72] 查看索引
来源：http://br.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://qe.huixiangedu.cn

[Q73] 查看表状态
来源：http://dr.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xg.jctech888.com.cn

[Q74] 强制使用索引
来源：http://xe.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bo.muxihuayi.cn

[Q75] 日期格式化
来源：http://cv.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dl.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mq.haigaiapp.cn

[Q76] 按天统计
来源：http://oh.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lj.muxihuayi.cn

[Q77] 时间加减
来源：http://bj.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kr.9csxet.cn

[Q78] 当前时间
来源：http://au.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://np.panjiajie.cn

[Q79] 字符串拼接
来源：http://ip.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zi.haigaiapp.cn

[Q80] 字符串截取
来源：http://am.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://co.yuexingan06.cn

[Q81] 字符串替换
来源：http://my.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fz.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://vl.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pc.wgjwhj.cn

[Q83] 大小写转换
来源：http://tx.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jv.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://mf.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ly.colortex.cn

[Q85] 数值取整
来源：http://sk.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yr.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://dj.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ul.nszjky.cn

[Q87] JSON 字段做条件
来源：http://uo.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pr.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://oe.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ly.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pj.lnxyls.cn

[Q89] 判断表是否存在
来源：http://bf.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://it.hahajie.cn

[Q90] 生成序号列
来源：http://jc.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ko.yuexingan06.cn

================================================================================
来源：http://et.haigaiapp.cn

R. Bash 专题
来源：http://eo.shxzukj.cn

================================================================================
来源：http://lz.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://vf.shxzukj.cn

#!/usr/bin/env bash
来源：http://oo.szsharing.cn

set -euo pipefail
来源：http://wf.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://km.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ba.haigaiapp.cn

[R03] 只读变量
来源：http://ot.jianghongdianzi.cn

readonly PI=3.14
来源：http://bd.jctech888.com.cn

[R04] 位置参数
来源：http://uh.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qt.szxytkj.cn

[R05] 参数默认值
来源：http://gi.lnxyls.cn

name="${1:-default}"
来源：http://ft.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://qm.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kn.colortex.cn

[R07] if 判断文件
来源：http://ic.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lk.panjiajie.cn

[R08] 数值比较
来源：http://lm.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bf.haigaiapp.cn

[R09] 字符串比较
来源：http://uu.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ul.haigaiapp.cn

[R10] 正则匹配
来源：http://ma.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fw.bookmarksfly.cn

[R11] case 多分支
来源：http://fx.shtwfgs.cn

case "$1" in
来源：http://ib.szsharing.cn

start) echo "启动" ;;
来源：http://ps.nszjky.cn

stop)  echo "停止" ;;
来源：http://yl.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://pk.haigaiapp.cn

esac
来源：http://ks.hahajie.cn

[R12] for 遍历文件
来源：http://rd.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://ad.shxzukj.cn

[R13] for 计数循环
来源：http://kv.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://ch.szsharing.cn

[R14] C 风格 for
来源：http://jr.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fx.huixiangedu.cn

[R15] while 逐行读文件
来源：http://md.szxytkj.cn


<!-- 参考信息 -->
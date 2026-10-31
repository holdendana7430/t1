代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hd.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ax.gzmigu.cn

[P03] 生成短随机字符串
来源：http://fu.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fk.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mv.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://up.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://he.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://be.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pc.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cr.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eb.bookmarksfly.cn

[P04] 求长度
来源：http://ax.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vm.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pq.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bm.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://fq.szsharing.cn

Go:   len(arr);  len(m)
来源：http://ty.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://gp.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fk.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://dj.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yo.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tp.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://js.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tl.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ye.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ah.shxzukj.cn

Ruby: a == b
来源：http://eb.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://so.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://am.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fh.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://wf.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://by.newstarts.cn

TS:   if (x == null) {}
来源：http://hd.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qv.gzmigu.cn

Go:   if x == nil {}
来源：http://ng.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sw.gzmigu.cn

C#:   if (x is null) {}
来源：http://xb.szsharing.cn

[P07] 防抖与节流
来源：http://bm.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ce.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://nl.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://st.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iy.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gy.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qk.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://me.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pg.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://st.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xy.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://im.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hl.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pu.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vi.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xd.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xz.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hm.asd995.cn

================================================================================
来源：http://ie.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hj.shxzukj.cn

================================================================================
来源：http://ml.haigaiapp.cn

[Q01] 创建表
来源：http://nk.yuexingan06.cn

CREATE TABLE users (
来源：http://jg.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oz.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://dm.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://si.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ml.wgjwhj.cn

);
来源：http://xy.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://xk.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://ij.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uw.nicolike.cn

user_id INT NOT NULL,
来源：http://zz.nszjky.cn

amount DECIMAL(10, 2),
来源：http://vc.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yh.chemitech.net.cn

);
来源：http://dp.lnxyls.cn

[Q03] 增加列
来源：http://cn.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yc.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://dx.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kx.huixiangedu.cn

[Q05] 重命名列
来源：http://ng.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xn.bjjhwx.cn

[Q06] 删除列
来源：http://nf.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cc.521024.cn

[Q07] 删除表
来源：http://hd.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://zp.panjiajie.cn

[Q08] 创建普通索引
来源：http://ys.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yl.9csxet.cn

[Q09] 创建唯一索引
来源：http://zq.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bc.huanxung.cn

[Q10] 插入单行
来源：http://nj.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tj.szsharing.cn

[Q11] 一次插入多行
来源：http://kf.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mb.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://ri.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gm.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ak.huanxung.cn

[Q13] 忽略重复插入
来源：http://ek.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qo.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://iw.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hd.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://za.gzmigu.cn

[Q15] 查询全部
来源：http://ou.muxihuayi.cn

SELECT * FROM users;
来源：http://kk.asd995.cn

[Q16] 查询指定列
来源：http://dk.bjjhwx.cn

SELECT id, name FROM users;
来源：http://dk.chemitech.net.cn

[Q17] 条件查询
来源：http://it.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nf.wgjwhj.cn

[Q18] 模糊匹配
来源：http://qo.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gb.jianghongdianzi.cn

[Q19] 范围查询
来源：http://ju.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cy.9csxet.cn

[Q20] IN 列表
来源：http://vh.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ol.muxihuayi.cn

[Q21] 空值判断
来源：http://xi.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hx.asd995.cn

[Q22] 排序
来源：http://cy.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lh.chemitech.net.cn

[Q23] 分页
来源：http://ah.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://io.asd995.cn

[Q24] 去重
来源：http://ju.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://sc.lnxyls.cn

[Q25] 只取前 N 条
来源：http://ao.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ru.jctech888.com.cn

[Q26] 计数
来源：http://fn.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://tg.yuexingan06.cn

[Q27] 条件计数
来源：http://nd.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sb.newstarts.cn

[Q28] 求和与平均
来源：http://bl.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ur.nicolike.cn

[Q29] 最大最小值
来源：http://ly.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ut.chemitech.net.cn

[Q30] 分组统计
来源：http://lp.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ps.huixiangedu.cn

[Q31] 分组后过滤
来源：http://sf.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xm.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://vg.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hu.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://il.9csxet.cn

[Q33] 多列分组
来源：http://us.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gq.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://qj.szxytkj.cn

SELECT * FROM (
来源：http://px.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sx.shxzskj.cn

) t WHERE rn = 1;
来源：http://ay.521024.cn

[Q35] 内连接
来源：http://rq.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qn.huanxung.cn

[Q36] 左连接
来源：http://kh.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kt.bjjhwx.cn

[Q37] 右连接
来源：http://gs.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tq.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wv.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ye.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://lw.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ox.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vh.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://il.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bc.gzmigu.cn

[Q41] 多表连接
来源：http://as.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dr.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://vk.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vv.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://jb.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://pw.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mg.jctech888.com.cn

[Q43] 标量子查询
来源：http://rj.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pf.bjjhwx.cn

[Q44] IN 子查询
来源：http://kn.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wi.521024.cn

[Q45] EXISTS 判断存在
来源：http://ki.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://of.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qk.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sx.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ra.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wh.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://et.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iz.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://uc.521024.cn

[Q49] 更新单行
来源：http://lp.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pk.wgjwhj.cn

[Q50] 批量更新
来源：http://tm.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yy.shxzukj.cn

[Q51] 用子查询更新
来源：http://xr.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jm.newstarts.cn

[Q52] 删除指定行
来源：http://cx.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://cb.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://gd.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bb.lnxyls.cn

[Q54] 清空表
来源：http://uo.colortex.cn

TRUNCATE TABLE logs;
来源：http://az.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://re.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ku.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://wq.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ab.hnjuh.cn

[Q57] 行号
来源：http://ie.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ne.shtwfgs.cn

[Q58] 累计求和
来源：http://sw.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qc.hnjuh.cn

[Q59] 分组内累计
来源：http://ih.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sj.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ux.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ds.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://af.bookmarksfly.cn

[Q61] 移动平均
来源：http://hi.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jw.szxytkj.cn

[Q62] 分组占比
来源：http://uu.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lj.lnxyls.cn

[Q63] 开启事务
来源：http://fa.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cw.jianghongdianzi.cn

[Q64] 提交事务
来源：http://kc.haigaiapp.cn

COMMIT;
来源：http://to.szxytkj.cn

[Q65] 回滚事务
来源：http://kp.huanxung.cn

ROLLBACK;
来源：http://mj.panjiajie.cn

[Q66] 行锁查询
来源：http://nv.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dx.panjiajie.cn

[Q67] 设置隔离级别
来源：http://vd.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mh.nszjky.cn

[Q68] 保存点
来源：http://vk.jctech888.com.cn

SAVEPOINT sp1;
来源：http://lb.colortex.cn

ROLLBACK TO sp1;
来源：http://xn.yuexingan06.cn

[Q69] 查看执行计划
来源：http://nj.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://by.yuexingan06.cn

[Q70] 更新统计信息
来源：http://fo.szsharing.cn

ANALYZE TABLE users;
来源：http://vz.nicolike.cn

[Q71] 查看建表语句
来源：http://of.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ah.bookmarksfly.cn

[Q72] 查看索引
来源：http://yf.9csxet.cn

SHOW INDEX FROM users;
来源：http://jc.wgjwhj.cn

[Q73] 查看表状态
来源：http://yg.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pe.lnxyls.cn

[Q74] 强制使用索引
来源：http://ov.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xn.asd995.cn

[Q75] 日期格式化
来源：http://kl.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fv.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ji.haigaiapp.cn

[Q76] 按天统计
来源：http://zw.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kt.yuntaijiaju.cn

[Q77] 时间加减
来源：http://uc.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://co.haigaiapp.cn

[Q78] 当前时间
来源：http://gq.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oa.lnxyls.cn

[Q79] 字符串拼接
来源：http://mu.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iu.chemitech.net.cn

[Q80] 字符串截取
来源：http://an.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zo.9csxet.cn

[Q81] 字符串替换
来源：http://no.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wz.asd995.cn

[Q82] 字符长度与字节长度
来源：http://fm.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xf.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://it.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vt.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://ri.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://lp.shtwfgs.cn

[Q85] 数值取整
来源：http://zt.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jl.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://lg.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ep.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://if.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ai.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://vf.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://af.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ah.nszjky.cn

[Q89] 判断表是否存在
来源：http://en.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yp.szsharing.cn

[Q90] 生成序号列
来源：http://go.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jz.szxytkj.cn

================================================================================
来源：http://le.yuexingan06.cn

R. Bash 专题
来源：http://va.wgjwhj.cn

================================================================================
来源：http://yl.521024.cn

[R01] shebang 与严格模式
来源：http://de.panjiajie.cn

#!/usr/bin/env bash
来源：http://tc.521024.cn

set -euo pipefail
来源：http://zi.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://vy.9csxet.cn

name="Tom"; echo "$name"
来源：http://el.shxzukj.cn

[R03] 只读变量
来源：http://ib.wgjwhj.cn

readonly PI=3.14
来源：http://ss.colortex.cn

[R04] 位置参数
来源：http://cj.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wz.asd995.cn

[R05] 参数默认值
来源：http://xf.huixiangedu.cn

name="${1:-default}"
来源：http://ft.521024.cn

[R06] 判断命令是否存在
来源：http://iy.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ct.newstarts.cn

[R07] if 判断文件
来源：http://pb.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sw.nicolike.cn

[R08] 数值比较
来源：http://oc.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xq.gzmigu.cn

[R09] 字符串比较
来源：http://eh.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xp.asd995.cn

[R10] 正则匹配
来源：http://hz.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dm.asd995.cn

[R11] case 多分支
来源：http://gd.hahajie.cn

case "$1" in
来源：http://bo.szsharing.cn

start) echo "启动" ;;
来源：http://vz.shxzukj.cn

stop)  echo "停止" ;;
来源：http://cm.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://uj.szxytkj.cn

esac
来源：http://ek.yuexingan06.cn

[R12] for 遍历文件
来源：http://hv.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://qn.hahajie.cn

[R13] for 计数循环
来源：http://sr.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://dt.chemitech.net.cn

[R14] C 风格 for
来源：http://ny.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zu.szsharing.cn

[R15] while 逐行读文件
来源：http://vs.huanxung.cn


<!-- 参考信息 -->